# Core Banking

## Documentation Overview

Core banking refers to the centralized computer systems that process and record all banking transactions across a bank's branches and channels. It connects every branch of a bank to a single, shared database, allowing customers to access their accounts from any location. This document covers the architecture, modules, transaction processing, and evolution of core banking systems.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the definition and purpose of core banking                     │
    │   Learn the architecture and components of core banking systems             │
    │   Study the major functional modules (CASA, loans, payments)                │
    │   Analyze transaction processing flow (OLTP vs batch)                       │
    │   Examine the role of the general ledger                                    │
    │   Understand the evolution from siloed to integrated systems                │
    │   Learn about core banking vendors and platforms                            │
    │   Study modern trends (cloud, APIs, real-time)                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Purpose

### What is Core Banking

Core banking is the back-end system that processes daily banking transactions and posts updates to accounts and other financial records. It is the central repository of customer account information and the engine that executes deposits, withdrawals, transfers, and loan payments.

How it works: A customer walks into any branch of their bank. The teller enters the transaction into the terminal. The terminal sends the request to the central core banking system. The system verifies the account exists, checks for sufficient funds (for withdrawals), updates the account balance, and records the transaction. The customer sees the updated balance immediately. The same system serves online banking, ATMs, mobile apps, and phone banking through different channels connected to the same core.

```
CORE BANKING SYSTEM POSITION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                         CHANNELS                                            │
    │                                                                             │
    │   ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐      │
    │   │ Branch   │  │   ATM    │  │ Online   │  │  Mobile  │  │ Call     │      │
    │   │ Teller   │  │          │  │ Banking  │  │   App    │  │ Center   │      │
    │   └────┬─────┘  └────┬─────┘  └────┬─────┘  └────┬─────┘  └────┬─────┘      │
    │        │             │             │             │             │            │
    │        └─────────────┴─────────────┼─────────────┴─────────────┘            │
    │                                    │                                        │
    │                                    ▼                                        │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                      CORE BANKING SYSTEM                            │   │
    │   │                                                                     │   │
    │   │  ┌─────────┐┌─────────┐┌───────────┐┌─────────┐┌─────────┐          │   │
    │   │  │Customer ││Account  ││Transaction││ Interest││ General │          │   │
    │   │  │ Master  ││ Ledger  ││ Engine    ││ Engine  ││ Ledger  │          │   │
    │   │  └─────────┘└─────────┘└───────────┘└─────────┘└─────────┘          │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                    │                                        │
    │                                    ▼                                        │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                    CENTRAL DATABASE                                 │   │
    │   │                                                                     │   │
    │   │  ┌─────────────────────────────────────────────────────────────┐    │   │
    │   │  │  Account  │ Customer │ Balance │ Transaction History        │    │   │
    │   │  │  Tables   │  Tables  │         │                            │    │   │
    │   │  └─────────────────────────────────────────────────────────────┘    │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Purpose of Core Banking

Core banking serves as the single source of truth for all customer account information and transaction records.

```
CORE BANKING PURPOSES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   PURPOSE                    │ DESCRIPTION                                  │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   Centralized Records        │ All customer accounts stored in one          │
    │                              │ central database accessible from any         │
    │                              │ branch or channel                            │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   Real-Time Processing       │ Transactions post instantly, balances        │
    │                              │ update immediately across all channels       │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   Single Customer View       │ All relationships with a customer            │
    │                              │ (checking, savings, loans, credit cards)     │
    │                              │ visible together                             │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   Transaction Integrity      │ Ensures every transaction is properly        │
    │                              │ recorded and accounted for                   │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   Regulatory Compliance      │ Provides audit trail and reporting for       │
    │                              │ regulators (AML, KYC, Basel)                 │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   Operational Efficiency     │ Automates manual processes, reduces          │
    │                              │ errors, lowers costs                         │
    │   ───────────────────────────│───────────────────────────────────────────── │
    │   ​Channel Integration        │ All channels (branch, ATM, online, mobile)   │
    │                              │ connect to same system                       │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Core Banking Architecture

### Three-Tier Architecture

Modern core banking systems use a three-tier architecture separating presentation, application logic, and data storage.

```
THREE-TIER ARCHITECTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TIER 1: PRESENTATION LAYER (Client)                                       │
    │                                                                             │
    │   ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐    │
    │   │ Teller       │  │ ATM Interface│  │ Web Browser  │  │ Mobile App   │    │
    │   │ Workstation  │  │              │  │              │  │              │    │
    │   └──────┬───────┘  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘    │
    │          │                 │                 │                 │            │
    │          └─────────────────┴────────┬────────┴─────────────────┘            │
    │                                     │                                       │
    │                                     │ API Calls / HTTPS                     │
    │                                     ▼                                       │
    │   TIER 2: APPLICATION LAYER (Business Logic)                                │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                         APPLICATION SERVER                          │   │
    │   │                                                                     │   │
    │   │  ┌───────────┐  ┌───────────┐  ┌───────────┐  ┌───────────┐         │   │
    │   │  │ Deposit   │  │ Withdrawal│  │ Transfer  │  │ Interest  │         │   │
    │   │  │ Module    │  │ Module    │  │ Module    │  │ Module    │         │   │
    │   │  └───────────┘  └───────────┘  └───────────┘  └───────────┘         │   │
    │   │                                                                     │   │
    │   │  ┌───────────┐  ┌───────────┐  ┌───────────┐  ┌───────────┐         │   │
    │   │  │ Loan      │  │ Interest  │  │ Customer  │  │ Reporting │         │   │
    │   │  │ Module    │  │ Accrual   │  │ Onboarding│  │ Module    │         │   │
    │   │  └───────────┘  └───────────┘  └───────────┘  └───────────┘         │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                      │                                      │
    │                                      │ SQL / Database Calls                 │
    │                                      ▼                                      │
    │   TIER 3: DATA LAYER (Storage)                                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                          DATABASE SERVER                            │   │
    │   │                                                                     │   │
    │   │  ┌─────────────────────────────────────────────────────────────┐    │   │
    │   │  │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │    │   │
    │   │  │  │ Account     │  │ Customer    │  │ Transaction │          │    │   │
    │   │  │  │ Table       │  │ Table       │  │ Table       │          │    │   │
    │   │  │  └─────────────┘  └─────────────┘  └─────────────┘          │    │   │
    │   │  │                                                             │    │   │
    │   │  │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │    │   │
    │   │  │  │ Loan Table  │  │ Interest    │  │ GL Table    │          │    │   │
    │   │  │  │             │  │ Rate Table  │  │             │          │    │   │
    │   │  │  └─────────────┘  └─────────────┘  └─────────────┘          │    │   │
    │   │  └─────────────────────────────────────────────────────────────┘    │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Online Transaction Processing (OLTP)

Core banking systems use Online Transaction Processing (OLTP) for real-time transaction execution. Each transaction is atomic, consistent, isolated, and durable (ACID).

How it works: A withdrawal request arrives. The system begins a database transaction. It locks the account record, reads the current balance, verifies sufficient funds, calculates the new balance, updates the record, writes a transaction log entry, and commits the changes. If any step fails, the entire transaction is rolled back. The account never shows an incorrect intermediate state.

```
ACID TRANSACTION PROPERTIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   PROPERTY     │ MEANING                        │ EXAMPLE                   │
    │   ─────────────│────────────────────────────────│───────────────────────────│
    │   Atomic       │ Transaction completes fully    │ Withdrawal either fully   │
    │                │ or not at all. No partial      │ completes or account      │
    │                │ updates.                       │ unchanged                 │
    │   ─────────────│────────────────────────────────│───────────────────────────│
    │   Consistent   │ Transaction leaves database    │ Balance never negative    │
    │                │ in valid state.                │ after withdrawal          │
    │   ─────────────│────────────────────────────────│───────────────────────────│
    │   Isolated     │ Concurrent transactions do     │ Two withdrawals from      │
    │                │ not interfere.                 │ same account do not       │
    │                │                                │ double-spend              │
    │   ─────────────│────────────────────────────────│───────────────────────────│
    │   Durable      │ Once committed, transaction    │ After confirmation,       │
    │                │ persists even after power      │ power loss does not       │
    │                │ failure.                       │ erase the withdrawal      │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Core Banking Modules

### Customer Information File (CIF)

The Customer Information File (CIF) is the central repository of all customer data. Each customer has a unique CIF number that links all their accounts and relationships.

```
CUSTOMER INFORMATION FILE STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER MASTER RECORD (CIF #12345678)                                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  DEMOGRAPHIC DATA                                                   │   │
    │   │  ├── Name: John Smith                                               │   │
    │   │  ├── Date of Birth: 1980-05-15                                      │   │
    │   │  ├── Tax ID (SSN): XXX-XX-1234                                      │   │
    │   │  ├── Address: 123 Main Street, Anytown, USA 12345                   │   │
    │   │  ├── Phone: (555) 123-4567                                          │   │
    │   │  └── Email: john.smith@email.com                                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  KYC / AML DATA                                                     │   │
    │   │  ├── ID Verification: Passport #ABC123, verified 2020-01-15       │   │
    │   │  ├── PEP Status: No                                                 │   │
    │   │  ├── Risk Rating: Medium                                            │   │
    │   │  ├── Source of Funds: Employment                                    │   │
    │   │  └── Last CDD Review: 2024-01-10                                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ACCOUNTS LINKED                                                    │   │
    │   │  ├── Account #1001: Checking (Primary)                              │   │
    │   │  ├── Account #1002: Savings                                         │   │
    │   │  ├── Account #1003: Money Market                                    │   │
    │   │  ├── Account #2001: Auto Loan                                       │   │
    │   │  └── Account #3001: Credit Card                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  RELATIONSHIP DATA                                                  │   │
    │   │  ├── Primary Banker: Jane Doe (Branch Manager)                      │   │
    │   │  ├── Customer Since: 2010-03-22                                     │   │
    │   │  ├── Total Relationship Value: $250,000                             │   │
    │   │  └── Product Preferences: Online banking, e-statements              │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Account Management Module

The account management module maintains all deposit accounts: checking, savings, money market, certificates of deposit.

```
ACCOUNT LEDGER STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ACCOUNT MASTER RECORD (#1001 - John Smith Checking)                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ACCOUNT ATTRIBUTES                                                 │   │
    │   │  ├── Account Type: Demand Deposit (Checking)                        │   │
    │   │  ├── Currency: USD                                                  │   │
    │   │  ├── Open Date: 2010-03-22                                          │   │
    │   │  ├── Status: Active                                                 │   │
    │   │  ├── Interest Rate: 0.00% (non-interest bearing)                    │   │
    │   │  └── Overdraft Protection: Yes (linked to Savings #1002)            │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CURRENT BALANCES                                                   │   │
    │   │  ├── Ledger Balance: $5,234.67                                      │   │
    │   │  ├── Available Balance: $5,234.67 (no holds)                        │   │
    │   │  ├── Collected Balance: $5,234.67                                   │   │
    │   │  └── Average Balance (30 days): $4,987.23                           │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LIMITS & CONTROLS                                                  │   │
    │   │  ├── Daily ATM Withdrawal Limit: $500                               │   │
    │   │  ├── Daily Debit Card Limit: $2,500                                 │   │
    │   │  ├── Per Transaction Limit: $5,000 (in-branch)                      │   │
    │   │  └── Minimum Balance Requirement: $0                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  FEE STRUCTURE                                                      │   │
    │   │  ├── Monthly Maintenance Fee: $10 (waived if balance > $1,500)      │   │
    │   │  ├── Overdraft Fee: $35                                             │   │
    │   │  ├── ATM Foreign Fee: $2.50                                         │   │
    │   │  └── Stop Payment Fee: $30                                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Transaction Processing Engine

The transaction processing engine handles all monetary movements between accounts. It validates, authorizes, posts, and logs each transaction.

```
TRANSACTION PROCESSING FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TRANSACTION REQUEST (Withdrawal $200 from Account #1001)                  │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 1: VALIDATION                                                        │
    │   ├── Account exists? Yes (#1001, John Smith Checking)                      │
    │   ├── Account active? Yes                                                   │
    │   ├── Transaction within limits? $200 < $500 (ATM limit)                    │
    │   └── Authentication verified? PIN correct                                  │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 2: AVAILABLE FUNDS CHECK                                             │
    │   ├── Current available balance: $5,234.67                                  │
    │   ├── Request amount: $200.00                                               │
    │   └── Result: SUFFICIENT FUNDS                                              │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 3: RESERVE FUNDS (Lock account)                                      │
    │   ├── Place hold on $200.00                                                 │
    │   ├── Available balance becomes $5,034.67 (temporarily)                     │
    │   └── Account locked for concurrent transactions                            │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 4: POST TRANSACTION                                                  │
    │   ├── Debit account: $5,234.67 → $5,034.67                                  │
    │   ├── Create transaction record: Withdrawal, $200, 2024-06-15 10:30:45      │
    │   ├── Update running balance                                                │
    │   └── Release account lock                                                  │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 5: UPDATE GENERAL LEDGER                                             │
    │   ├── Debit: Customer Deposits (Liability) -$200                            │
    │   └── Credit: Vault Cash (Asset) -$200 (if cash) or                         │
    │            Settlement Account (if electronic)                               │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 6: CONFIRMATION                                                      │
    │   ├── Generate receipt                                                      │
    │   ├── Send notification (optional)                                          │
    │   └── Return success to channel                                             │
    │        │                                                                    │
    │        ▼                                                                    │
    │   TRANSACTION COMPLETE                                                      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Loans Module

The loans module manages the entire loan lifecycle: origination, disbursement, repayment, collection, and write-off.

```
LOAN LIFECYCLE IN CORE BANKING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   PHASE 1: ORIGINATION                                                      │
    │   ├── Application received and entered                                      │
    │   ├── Credit check (internal and external bureaus)                          │
    │   ├── Underwriting (Five C's analysis)                                      │
    │   ├── Approval (auto-decision or manual)                                    │
    │   └── Loan terms set (amount, rate, term, payment schedule)                 │
    │        │                                                                    │
    │        ▼                                                                    │
    │   PHASE 2: DISBURSEMENT                                                     │
    │   ├── Create loan account in core system                                    │
    │   ├── Set up amortization schedule                                          │
    │   ├── Disburse funds (credit to customer deposit account)                   │
    │   └── Loan appears on customer's statement                                  │
    │        │                                                                    │
    │        ▼                                                                    │
    │   PHASE 3: SERVICING                                                        │
    │   ├── Automatic payment posting (ACH, check, card)                          │
    │   ├── Interest accrual calculation (daily or monthly)                       │
    │   ├── Late fee assessment (if payment missed)                               │
    │   ├── Principal and interest allocation                                     │
    │   └── Amortization schedule tracking                                        │
    │        │                                                                    │
    │        ├─────────────────────────────────────────────────────┐              │
    │        │                                                     │              │
    │        ▼                                                     ▼              │
    │   IF CURRENT                                         IF PAST DUE            │
    │   ├── Continue normal servicing                     ├── Send notices        │
    │   ├── Report to credit bureaus                      ├── Assess late fees    │
    │   └── Release collateral (when paid off)            ├── Call customer       │
    │                                                      └── Report delinquency │
    │                                                             │               │
    │                                                             ▼               │
    │                                                      IF DEFAULT             │
    │                                                      ├── Accelerate loan    │
    │                                                      ├── Charge-off         │
    │                                                      └── Collections        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Interest Engine

The interest engine calculates interest on deposits and loans according to complex rules: different rates for different products, tiered rates, compounding frequencies.

```
INTEREST CALCULATION TYPES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DEPOSIT INTEREST (Bank pays customer)                                     │
    │                                                                             │
    │   Simple Interest: I = P × r × t                                            │
    │   └── Used for short-term deposits (under 1 year)                           │
    │                                                                             │
    │   Compound Interest: A = P × (1 + r/n)^(n×t)                                │
    │   └── Used for savings accounts, CDs                                        │
    │                                                                             │
    │   Daily Balance Method: Interest = Σ (Daily Balance × Daily Rate)           │
    │   └── Most common for checking and savings                                  │
    │                                                                             │
    │   Average Daily Balance: Interest = (Sum of daily balances / Days) × Rate   │
    │   └── Used by some credit unions                                            │
    │                                                                             │
    │                                                                             │
    │   LOAN INTEREST (Customer pays bank)                                        │
    │                                                                             │
    │   Simple Interest (Consumer loans): I = P × r × t                           │
    │                                                                             │
    │   Amortizing (Mortgage): Equal payments, changing interest/principal split  │
    │                                                                             │
    │   Rule of 78 (Precomputed): Interest front-loaded, prohibited in many       │
    │   jurisdictions                                                             │
    │                                                                             │
    │   Daily Accrual: Interest accrues daily, posted monthly                     │
    │   └── Standard for most loans                                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## End of Day (EOD) Processing

### Batch Processing Cycle

While transactions post in real-time during the day, many calculations and updates happen in overnight batch processing.

```
END OF DAY (EOD) PROCESSING FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DAYTIME (6:00 AM - 10:00 PM)                                              │
    │   ├── Real-time OLTP transactions                                           │
    │   ├── Online balances update instantly                                      │
    │   └── Transaction log accumulates                                           │
    │        │                                                                    │
    │        ▼                                                                    │
    │   CUTOVER (10:00 PM)                                                        │
    │   ├── Stop accepting new transactions                                       │
    │   ├── Flush remaining transactions from queues                              │
    │   └── System enters maintenance mode                                        │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 1: ACCRUE INTEREST                                                   │
    │   ├── Calculate daily interest on all deposit accounts                      │
    │   ├── Calculate daily interest accrual on all loans                         │
    │   └── Post accrual entries to ledgers                                       │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 2: APPLY FEES                                                        │
    │   ├── Monthly maintenance fees (on appropriate day)                         │
    │   ├── Overdraft fees (from daytime events)                                  │
    │   ├── Late payment fees (on loans)                                          │
    │   └── Inactivity fees                                                       │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 3: PROCESS AUTOMATIC PAYMENTS                                        │
    │   ├── ACH credits (payroll direct deposits)                                 │
    │   ├── ACH debits (loan payments, bill pay)                                  │
    │   ├── Internal transfers (sweep accounts)                                   │
    │   └── Maturity rollovers (CDs)                                              │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 4: UPDATE ACCOUNT STATUS                                             │
    │   ├── Flag overdrawn accounts                                               │
    │   ├── Update past due status on loans                                       │
    │   ├── Close matured CDs                                                     │
    │   └── Activate new accounts                                                 │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 5: RECONCILE WITH GENERAL LEDGER                                     │
    │   ├── Sum all deposit account balances                                      │
    │   ├── Compare to GL control account                                         │
    │   ├── Investigate discrepancies                                             │
    │   └── Post adjusting entries if needed                                      │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 6: GENERATE REPORTS                                                  │
    │   ├── Customer statements                                                   │
    │   ├── Regulatory reports (Fed, FDIC)                                        │
    │   ├── Internal management reports                                           │
    │   └── Exception reports                                                     │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 7: DATABASE BACKUP                                                   │
    │   ├── Full backup of all databases                                          │
    │   ├── Archive transaction logs                                              │
    │   └── Replicate to disaster recovery site                                   │
    │        │                                                                    │
    │        ▼                                                                    │
    │   SYSTEM RESUMES (6:00 AM)                                                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## General Ledger Integration

### Double-Entry Posting

Every customer transaction also posts to the bank's general ledger, maintaining the accounting equation.

```
GL INTEGRATION EXAMPLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER DEPOSITS $1000 CASH (Branch transaction)                         │
    │                                                                             │
    │   CORE BANKING CUSTOMER LEDGER:                                             │
    │   ├── Customer A deposit account: +$1,000 (Credit)                          │
    │   └── Vault Cash: +$1,000 (Debit)                                           │
    │        │                                                                    │
    │        ▼                                                                    │
    │   GENERAL LEDGER POSTING:                                                   │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                       │ Debit ($)    │ Credit ($)          │   │
    │   │  ──────────────────────────────│──────────────│─────────────────────│   │
    │   │  Vault Cash (Asset)            │ 1,000        │                     │   │
    │   │  Customer Deposits (Liability) │              │ 1,000               │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   CUSTOMER TRANSFERS $500 BETWEEN ACCOUNTS                                  │
    │                                                                             │
    │   CORE BANKING CUSTOMER LEDGER:                                             │
    │   ├── Customer A Checking: -$500 (Debit)                                    │
    │   └── Customer A Savings: +$500 (Credit)                                    │
    │        │                                                                    │
    │        ▼                                                                    │
    │   GENERAL LEDGER POSTING:                                                   │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                      │ Debit ($)    │ Credit ($)           │   │
    │   │  ─────────────────────────────│──────────────│──────────────────────│   │
    │   │  Checking Deposits (Liability)│ 500          │                      │   │
    │   │  Savings Deposits (Liability) │              │ 500                  │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Note: Total liabilities unchanged.                                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Suspense and Clearing Accounts

Suspense accounts temporarily hold transactions that cannot be fully processed, pending investigation or completion.

```
SUSPENSE ACCOUNT USAGE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   EXAMPLE: ATM Deposit with envelope (amount unknown)                       │
    │                                                                             │
    │   STEP 1: Customer deposits envelope at ATM, claims $200                    │
    │   ├── Debit: ATM Cash (Asset) -$200 (envelope removed)                      │
    │   └── Credit: ATM Suspense (Liability) +$200                                │
    │                                                                             │
    │   STEP 2: Bank processes envelope next day, finds $150                      │
    │   ├── Debit: ATM Suspense (Liability) -$200 (reverse)                       │
    │   └── Credit: ATM Suspense (Liability) +$150 (correct)                      │
    │                                                                             │
    │   STEP 3: Adjust customer account                                           │
    │   ├── Debit: Customer Deposits (Liability) -$50 (reduce by $50)             │
    │   └── Credit: ATM Suspense (Liability) -$150 (close suspense)               │
    │                                                                             │
    │   Suspense accounts are zeroed out after investigation.                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Evolution of Core Banking

### Generations of Core Banking Systems

```
CORE BANKING GENERATIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   GENERATION 1: BRANCH AUTOMATION (1970s-1980s)                            │
    │   ├── Standalone systems per branch                                        │
    │   ├── No real-time connection between branches                            │
    │   ├── Batch processing overnight                                          │
    │   ├── No customer access outside branch                                   │
    │   └── Example: IBM mainframe with branch terminals                        │
    │                                                                             │
    │                                                                             │
    │   GENERATION 2: ONLINE REAL-TIME (1990s-2000s)                            │
    │   ├── Centralized database connecting all branches                        │
    │   ├── Real-time transaction processing (OLTP)                             │
    │   ├── ATM networks integrated                                             │
    │   ├── Early online banking (dial-up)                                      │
    │   └── Example: FIS Profile, Fiserv Signature                             │
    │                                                                             │
    │                                                                             │
    │   GENERATION 3: MULTI-CHANNEL (2000s-2010s)                               │
    │   ├── Single core serving all channels                                    │
    │   ├── Internet banking, mobile apps, call centers                         │
    │   ├── API layers for channel integration                                  │
    │   ├── Customer relationship management (CRM) integrated                   │
    │   └── Example: Temenos T24, Oracle Flexcube                              │
    │                                                                             │
    │                                                                             │
    │   GENERATION 4: MODULAR / CLOUD (2010s-present)                          │
    │   ├── Microservices architecture (independent modules)                   │
    │   ├── Cloud-native (AWS, Azure, GCP)                                      │
    │   ├── Real-time payments (FedNow, UPI, Pix)                               │
    │   ├── Open banking APIs (PSD2, consumer data rights)                      │
    │   ├── AI / Machine learning integration                                   │
    │   └── Examples: Thought Machine Vault, Mambu, 10x Banking                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Legacy vs Modern Core Banking

```
LEGACY VS MODERN COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FEATURE              │ LEGACY CORE          │ MODERN CORE                │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Architecture         │ Monolithic           │ Microservices             │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Deployment           │ On-premise           │ Cloud-native              │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Technology           │ COBOL, Assembler     │ Java, Go, Python, .NET    │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Database             │ Hierarchical (IMS),  │ Relational (PostgreSQL,    │
    │                        │ VSAM                 │ Oracle), NoSQL            │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Processing           │ Batch (overnight)    │ Real-time (24/7)          │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Downtime for         │ Hours (EOD batch)    │ Seconds (rolling updates) │
    │   maintenance          │                      │                           │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   New product          │ Months               │ Days to weeks             │
    │   time to market       │                      │                           │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Scalability          │ Vertical (bigger     │ Horizontal (add servers)  │
    │                        │ mainframe)           │                           │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   API capabilities     │ Limited, custom      │ Native REST APIs          │
    │   ─────────────────────│──────────────────────│────────────────────────────│
    │   Cost structure       │ High fixed (licenses,│ Variable (pay-as-you-go)  │
    │                        │ hardware)            │                           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Major Core Banking Vendors

```
VENDOR LANDSCAPE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   VENDOR                │ PRODUCT(S)           │ TYPICAL CUSTOMERS         │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Temenos              │ T24 (Transact)        │ Global, large banks       │
    │                        │ Infinity             │                           │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   FIS                  │ Profile, IBS,        │ Regional banks, US        │
    │                        │ Horizon              │                           │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Fiserv               │ Signature, Premier,  │ Community banks, credit   │
    │                        │ DNA                  │ unions                    │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Jack Henry           │ SilverLake, CIF 20/20│ US community banks        │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Oracle               │ Flexcube             │ Large, international      │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Finastra             │ Fusion Essence,       │ Mid-size banks            │
    │                        │ Equation             │                           │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Thought Machine      │ Vault                │ Challenger banks, cloud-  │
    │                        │                      │ native adopters          │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   Mambu                │ Mambu Cloud Core     │ Digital banks, fintechs   │
    │   ──────────────────────│──────────────────────│───────────────────────────│
    │   10x Banking          │ SuperCore            │ UK, Australian banks      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Security and Access Control

### User Roles and Permissions

Core banking systems implement granular access controls based on job roles.

```
ACCESS CONTROL LAYERS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ROLE LAYER 1: TELLER                                                     │
    │   ├── Can view: Customer basic info, account balances                      │
    │   ├── Can do: Cash deposits, withdrawals, transfers                        │
    │   ├── Cannot do: Open accounts, modify limits, approve loans              │
    │   └── Requires supervisor override for transactions > $10,000             │
    │                                                                             │
    │   ROLE LAYER 2: CUSTOMER SERVICE REPRESENTATIVE (CSR)                      │
    │   ├── Can do: All teller functions                                        │
    │   ├── Plus: Open accounts, order checks, change addresses                 │
    │   ├── Cannot do: Approve loans, override limits                           │
    │   └── Requires manager override for certain operations                    │
    │                                                                             │
    │   ROLE LAYER 3: BRANCH MANAGER                                             │
    │   ├── Can do: All CSR functions                                           │
    │   ├── Plus: Approve overrides, approve loans up to $50,000                │
    │   ├── Cannot do: Access other branches without authorization             │
    │   └── Can override most teller and CSR limits                             │
    │                                                                             │
    │   ROLE LAYER 4: OPERATIONS / BACK OFFICE                                   │
    │   ├── Can view: All accounts (no geographical restrictions)               │
    │   ├── Can do: Adjust entries, reverse transactions                        │
    │   ├── Cannot do: Access customer passwords, PCI data                      │
    │   └── All actions logged and audited                                      │
    │                                                                             │
    │   ROLE LAYER 5: SYSTEM ADMINISTRATOR                                       │
    │   ├── Can do: Create users, assign roles, system configuration           │
    │   ├── Cannot do: View customer data (segregation of duties)              │
    │   └── Requires second admin for critical changes                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Audit Trail

Every transaction and access event is logged for security, compliance, and forensic purposes.

```
AUDIT LOG ENTRY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   AUDIT RECORD #: 20240615103045-0001                                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Timestamp: 2024-06-15 10:30:45.123 UTC                             │   │
    │   │  Event Type: WITHDRAWAL                                              │   │
    │   │  User ID: TELLER_JSMITH (Jane Smith, Teller, Branch #101)           │   │
    │   │  Terminal ID: B101-T03 (Branch 101, Teller Station 3)               │   │
    │   │  Session ID: SESS-8F3A2B1C                                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account: 1001 (John Smith Checking)                                │   │
    │   │  Action: Debit $200.00                                              │   │
    │   │  Balance Before: $5,234.67                                          │   │
    │   │  Balance After: $5,034.67                                           │   │
    │   │  Authorization: PIN verified (token AUTH-789XYZ)                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Digital Signature: 0x7F3A2B1C9D4E8F5A6B2C3D4E5F6A7B8C9D0E1F2A3B4C   │   │
    │   │  Hash (SHA-256): 3F4A2B1C8D9E0F1A2B3C4D5E6F7A8B9C0D1E2F3A4B5C6D7E   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Audit logs are immutable and stored for 7+ years.                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
CORE BANKING FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Available Balance = Ledger Balance - Holds - Uncleared Items            │
    │                                                                             │
    │   Daily Interest (Simple) = Principal × (Annual Rate / 365)               │
    │                                                                             │
    │   Daily Interest (Compound) = Principal × (1 + r/365)^(n) - Principal     │
    │                                                                             │
    │   Loan Payment (Amortizing) = P × [r(1+r)^n] / [(1+r)^n - 1]              │
    │   (P = principal, r = monthly rate, n = number of payments)              │
    │                                                                             │
    │   Average Daily Balance = Σ(Daily Balance) / Days in Period               │
    │                                                                             │
    │   Interest Accrued = Average Daily Balance × Rate × Days / 365            │
    │                                                                             │
    │   Late Fee = Minimum (Max Fee, Interest Rate × Past Due Amount)          │
    │                                                                             │
    │   Overdraft Fee Applied If: Available Balance < Withdrawal Amount         │
    │                                                                             │
    │   GL Control Account Balance = Σ(Subsidiary Ledger Balances)              │
    │                                                                             │
    │   Transaction Throughput = Transactions per Second (TPS)                  │
    │   Typical core banking: 500-5000 TPS                                     │
    │                                                                             │
    │   Batch Processing Window = End of Day cutoff to system resume            │
    │   Typical: 4-6 hours                                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Core banking is the central system that processes all banking transactions and maintains account records.

2. Three-tier architecture: Presentation (channels), Application (business logic), Data (database).

3. OLTP (Online Transaction Processing) enables real-time transactions with ACID properties.

4. ACID: Atomic, Consistent, Isolated, Durable. Ensures transaction integrity.

5. Customer Information File (CIF) is central repository of all customer data with unique CIF number.

6. Account module maintains deposit accounts: checking, savings, money market, CDs.

7. Transaction engine validates, authorizes, posts, and logs each transaction.

8. Loans module manages origination, disbursement, servicing, collection, write-off.

9. Interest engine calculates deposit interest and loan interest using daily balance method.

10. End of Day (EOD) batch processing: accrue interest, apply fees, process ACH, update status, reconcile GL, generate reports, backup.

11. GL integration ensures every customer transaction posts to general ledger with double-entry.

12. Suspense accounts temporarily hold transactions pending investigation or completion.

13. Evolution: Branch automation (1970s) → Online real-time (1990s) → Multi-channel (2000s) → Modular/Cloud (2010s+).

14. Legacy core: monolithic, COBOL, batch processing, on-premise, expensive.

15. Modern core: microservices, cloud-native, real-time, API-first, scalable.

16. Major vendors: Temenos, FIS, Fiserv, Jack Henry, Oracle, Finastra, Thought Machine, Mambu, 10x Banking.

17. Access control: role-based with teller, CSR, manager, operations, admin layers.

18. Audit trail: every transaction logged with timestamp, user, terminal, before/after balances, digital signature.

19. Audit logs are immutable and stored for regulatory compliance (7+ years).

20. Core banking is the single source of truth for all customer accounts and transactions.

*This documentation belongs to https://github.com/InterCentury*
