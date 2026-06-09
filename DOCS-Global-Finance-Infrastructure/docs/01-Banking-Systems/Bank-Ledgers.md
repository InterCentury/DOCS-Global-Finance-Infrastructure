# Bank Ledgers

## Documentation Overview

A bank ledger is the fundamental record-keeping system that tracks all financial transactions, account balances, and ownership of funds within a banking institution. It is the single source of truth for who owns what, who owes what, and what transactions have occurred. This document covers the structure, operation, types, and modern evolution of bank ledgers from physical books to distributed ledger technology.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the fundamental purpose of bank ledgers                        │
    │   Learn double-entry bookkeeping mechanics                                  │
    │   Study the structure of general ledger and subsidiary ledgers              │
    │   Analyze the role of ledgers in money creation                             │
    │   Examine the distinction between bank money and central bank money         │
    │   Understand ledger reconciliation processes                                │
    │   Learn the evolution from physical to digital ledgers                      │
    │   Study distributed ledger technology and its applications                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Purpose

### What is a Bank Ledger

A bank ledger is the official record of all financial transactions and account balances maintained by a bank. It is the definitive record of deposits, withdrawals, loans, and transfers. Every penny held by or owed to the bank is recorded in its ledger system.

How it works: When a customer deposits $100, the bank ledger records a debit (increase) to the bank's cash asset and a credit (increase) to the customer's deposit liability. When a customer transfers $50 to another account, the ledger debits one account and credits another. The ledger must always balance: total assets always equal total liabilities plus equity.

```
BANK LEDGER FUNDAMENTAL IDENTITY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   THE ACCOUNTING EQUATION:                                                  │
    │                                                                             │
    │   ASSETS = LIABILITIES + EQUITY                                             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ASSETS (What the bank owns)                                       │   │
    │   │   ├── Cash and reserves at central bank                             │   │
    │   │   ├── Loans made to customers                                       │   │
    │   │   ├── Securities held (bonds, treasuries)                           │   │
    │   │   ├── Physical assets (buildings, equipment)                        │   │
    │   │   └── Other assets                                                  │   │
    │   │                                                                     │   │
    │   │   LIABILITIES (What the bank owes)                                  │   │
    │   │   ├── Customer deposits (checking, savings, CDs)                    │   │
    │   │   ├── Borrowings from other banks                                   │   │
    │   │   └── Other liabilities                                             │   │
    │   │                                                                     │   │
    │   │   EQUITY (Owner's stake)                                            │   │
    │   │   ├── Shareholder capital                                           │   │
    │   │   ├── Retained earnings                                             │   │
    │   │   └── Other equity accounts                                         │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Every transaction affects at least two accounts. The ledger must          │
    │   always satisfy this equation.                                             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Purpose of Bank Ledgers

The bank ledger serves multiple critical functions in the financial system.

```
LEDGER FUNCTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FUNCTION                │ DESCRIPTION                                     │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Record Keeping          │ Maintains permanent record of all              │
    │                          │ transactions and balances                       │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Ownership Tracking      │ Determines who owns what funds                 │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Transfer Execution      │ Enables movement of funds between accounts     │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Balance Verification    │ Confirms available funds for spending          │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Regulatory Reporting    │ Provides data for central bank and             │
    │                          │ regulatory oversight                            │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Fraud Detection         │ Enables identification of unauthorized         │
    │                          │ transactions                                    │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Audit Trail             │ Provides evidence for audits and               │
    │                          │ investigations                                   │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Interest Calculation    │ Computes interest earned or owed on accounts   │
    │   ────────────────────────│─────────────────────────────────────────────────│
    │   Financial Statement     │ Feeds into bank's income statement and         │
    │   Preparation             │ balance sheet                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Double-Entry Bookkeeping

### The Fundamental Mechanism

Double-entry bookkeeping is the system where every transaction is recorded as both a debit and a credit in at least two accounts. The total debits must always equal total credits.

How it works: Developed by Luca Pacioli in 1494, double-entry ensures the accounting equation always balances. A debit (dr) increases asset or expense accounts and decreases liability, equity, or revenue accounts. A credit (cr) increases liability, equity, or revenue accounts and decreases asset or expense accounts.

```
DOUBLE-ENTRY RULES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ACCOUNT TYPE        │ DEBIT (dr) EFFECT    │ CREDIT (cr) EFFECT          │
    │   ────────────────────│──────────────────────│─────────────────────────────│
    │   Assets              │ Increase (+)         │ Decrease (-)                │
    │   ────────────────────│──────────────────────│─────────────────────────────│
    │   Liabilities         │ Decrease (-)         │ Increase (+)                │
    │   ────────────────────│──────────────────────│─────────────────────────────│
    │   Equity              │ Decrease (-)         │ Increase (+)                │
    │   ────────────────────│──────────────────────│─────────────────────────────│
    │   Income/Revenue      │ Decrease (-)         │ Increase (+)                │
    │   ────────────────────│──────────────────────│─────────────────────────────│
    │   Expenses            │ Increase (+)         │ Decrease (-)                │
    │                                                                             │
    │                                                                             │
    │   MEMORY AID:                                                              │
    │   DEAD CLIC: Debits = Expenses + Assets + Drawings (Dividends)            │
    │             Credits = Liabilities + Income + Capital                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Transaction Examples

```
BANK TRANSACTION LEDGER ENTRIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   EXAMPLE 1: Customer deposits $1000 cash                                 │
    │                                                                             │
    │   Account                    │ Debit ($)    │ Credit ($)                   │
    │   ───────────────────────────│──────────────│──────────────────────────────│
    │   Cash (Asset)               │ 1,000        │                              │
    │   Customer Deposits (Liability)│            │ 1,000                        │
    │                                                                             │
    │   Explanation: Bank receives cash (asset increases) and incurs a deposit   │
    │   liability to customer (liability increases).                             │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE 2: Bank makes $5000 loan to customer                            │
    │                                                                             │
    │   Account                    │ Debit ($)    │ Credit ($)                   │
    │   ───────────────────────────│──────────────│──────────────────────────────│
    │   Loans Receivable (Asset)   │ 5,000        │                              │
    │   Customer Deposit (Liability)│            │ 5,000                         │
    │                                                                             │
    │   Explanation: Bank creates a loan asset and credits the customer's       │
    │   deposit account (new money creation).                                   │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE 3: Customer transfers $200 to another customer                   │
    │                                                                             │
    │   Account                    │ Debit ($)    │ Credit ($)                   │
    │   ───────────────────────────│──────────────│──────────────────────────────│
    │   Customer A Deposits        │ 200          │                              │
    │   (Liability)                │              │                              │
    │   Customer B Deposits        │              │ 200                          │
    │   (Liability)                │              │                              │
    │                                                                             │
    │   Explanation: One liability account decreases, another increases.        │
    │   Total liabilities unchanged.                                             │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE 4: Bank pays $1000 interest to depositors                        │
    │                                                                             │
    │   Account                    │ Debit ($)    │ Credit ($)                   │
    │   ───────────────────────────│──────────────│──────────────────────────────│
    │   Interest Expense           │ 1,000        │                              │
    │   (Equity reduction)         │              │                              │
    │   Customer Deposits (Liability)│            │ 1,000                        │
    │                                                                             │
    │   Explanation: Expense reduces equity; liability to customer increases.   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Ledger Structure

### General Ledger

The general ledger is the master set of accounts that summarizes all transactions recorded in subsidiary ledgers. It contains control accounts for each major category.

How it works: The general ledger includes control accounts for assets, liabilities, equity, revenue, and expenses. Individual customer balances are not recorded here; instead, a single control account (e.g., "Customer Deposits") shows the total of all individual deposit accounts. Subsidiary ledgers contain the detailed individual records.

```
GENERAL LEDGER STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   GENERAL LEDGER (Summary level)                                           │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ASSETS                                                             │   │
    │   │  ├── Cash Control Account: $50,000,000                             │   │
    │   │  ├── Loans Control Account: $500,000,000                           │   │
    │   │  ├── Securities Control Account: $200,000,000                      │   │
    │   │  └── Reserves at Central Bank: $30,000,000                         │   │
    │   │                                                                     │   │
    │   │  LIABILITIES                                                        │   │
    │   │  ├── Customer Deposits Control: $600,000,000                       │   │
    │   │  ├── Borrowings Control: $100,000,000                              │   │
    │   │  └── Other Liabilities: $50,000,000                                │   │
    │   │                                                                     │   │
    │   │  EQUITY                                                             │   │
    │   │  ├── Share Capital: $20,000,000                                    │   │
    │   │  └── Retained Earnings: $10,000,000                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Total Assets ($780M) = Total Liabilities + Equity ($780M)               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Subsidiary Ledgers

Subsidiary ledgers contain the detailed individual records for each control account. They provide the granular transaction-level detail.

How it works: Each control account in the general ledger has a corresponding subsidiary ledger. The subsidiary ledger contains individual records (accounts) for each customer, each loan, each security, etc. The sum of all subsidiary ledger balances equals the control account balance in the general ledger.

```
SUBSIDIARY LEDGER STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   GENERAL LEDGER                     SUBSIDIARY LEDGERS                    │
    │   (Control Accounts)                 (Detail Records)                      │
    │                                                                             │
    │   ┌─────────────────────┐            ┌─────────────────────────────────┐   │
    │   │ Customer Deposits   │            │ Customer A: $5,000              │   │
    │   │ Control: $600M      │◄───────────│ Customer B: $12,000             │   │
    │   │                     │            │ Customer C: $3,400              │   │
    │   │                     │            │ Customer D: $22,500             │   │
    │   │                     │            │ ... (100,000 customers)         │   │
    │   │                     │            │ Total: $600,000,000              │   │
    │   └─────────────────────┘            └─────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────┐            ┌─────────────────────────────────┐   │
    │   │ Loans Control:      │            │ Loan 1001: $250,000              │   │
    │   │ $500M               │◄───────────│ Loan 1002: $75,000               │   │
    │   │                     │            │ Loan 1003: $500,000              │   │
    │   │                     │            │ Loan 1004: $125,000              │   │
    │   │                     │            │ ... (50,000 loans)               │   │
    │   │                     │            │ Total: $500,000,000              │   │
    │   └─────────────────────┘            └─────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────┐            ┌─────────────────────────────────┐   │
    │   │ Reserves Control:   │            │ Account at Central Bank:        │   │
    │   │ $30M                │◄───────────│ $30,000,000 (single account)    │   │
    │   └─────────────────────┘            └─────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Customer Account Ledger

The customer account ledger is the subsidiary ledger that tracks individual customer deposits and transactions. This is what customers see as their bank balance.

How it works: Each customer has a unique account record. Every deposit increases the customer's balance (credit to the customer's liability account from the bank's perspective). Every withdrawal decreases the balance (debit). The ledger maintains a running balance and transaction history.

```
CUSTOMER ACCOUNT LEDGER EXAMPLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Account Number: 12345678                                                 │
    │   Account Holder: John Smith                                               │
    │   Account Type: Checking                                                   │
    │                                                                             │
    │   Date        │ Description        │ Debit ($) │ Credit ($) │ Balance ($)  │
    │   ────────────│────────────────────│───────────│────────────│──────────────│
    │   2024-01-01  │ Opening Balance    │           │            │ 5,000.00     │
    │   2024-01-03  │ Direct Deposit     │           │ 2,000.00   │ 7,000.00     │
    │               │ (Payroll)          │           │            │              │
    │   2024-01-05  │ ATM Withdrawal     │ 200.00    │            │ 6,800.00     │
    │   2024-01-07  │ Check #1001        │ 150.00    │            │ 6,650.00     │
    │   2024-01-10  │ Debit Card Purchase│ 45.50     │            │ 6,604.50     │
    │   2024-01-15  │ Transfer to Savings│ 500.00    │            │ 6,104.50     │
    │   2024-01-20  │ Interest Credit    │           │ 5.25       │ 6,109.75     │
    │   2024-01-25  │ Online Payment     │ 800.00    │            │ 5,309.75     │
    │   2024-01-31  │ Monthly Fee        │ 10.00     │            │ 5,299.75     │
    │                                                                             │
    │   Bank's perspective: This is a liability account. Credit increases      │
    │   the bank's obligation to the customer. Debit decreases it.              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Transaction Processing

### Deposit Processing

When a customer makes a deposit, multiple ledger entries are created across different accounts.

```
DEPOSIT PROCESSING FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER DEPOSITS $1000 CASH                                             │
    │        │                                                                   │
    │        ▼                                                                   │
    │   TELLER ENTERS TRANSACTION INTO BANK SYSTEM                               │
    │        │                                                                   │
    │        ▼                                                                   │
    │   LEDGER UPDATES:                                                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  SUBSIDIARY LEDGER (Customer Account)                               │   │
    │   │  ├── Customer 12345: +$1,000 (Credit)                               │   │
    │   │                                                                     │   │
    │   │  GENERAL LEDGER                                                     │   │
    │   │  ├── Customer Deposits Control: +$1,000 (Credit)                    │   │
    │   │  └── Cash on Hand Control: +$1,000 (Debit)                          │   │
    │   │                                                                     │   │
    │   │  VAULT CASH LEDGER (Physical tracking)                              │   │
    │   │  ├── Vault Cash Count: +$1,000                                      │   │
    │   │  └── Serial number tracking (if required)                           │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   RECONCILIATION: Customer account balance matches transaction history    │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Transfer Processing

A transfer between accounts at the same bank is a simple internal ledger adjustment.

How it works: The sending account is debited (decreased). The receiving account is credited (increased). The bank's total liabilities remain unchanged. No external settlement is needed.

```
INTERNAL TRANSFER PROCESSING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER A TRANSFERS $500 TO CUSTOMER B (Same bank)                      │
    │                                                                             │
    │   BEFORE TRANSFER:                                                         │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Customer A Deposit (Liability): $10,000                            │   │
    │   │  Customer B Deposit (Liability): $5,000                             │   │
    │   │  Total Customer Deposits: $15,000                                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   LEDGER ENTRIES:                                                          │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                    │ Debit ($)    │ Credit ($)              │   │
    │   │  ───────────────────────────│──────────────│─────────────────────────│   │
    │   │  Customer A Deposit         │ 500          │                         │   │
    │   │  Customer B Deposit         │              │ 500                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   AFTER TRANSFER:                                                          │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Customer A Deposit (Liability): $9,500                             │   │
    │   │  Customer B Deposit (Liability): $5,500                             │   │
    │   │  Total Customer Deposits: $15,000 (unchanged)                       │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Key insight: Total bank liabilities unchanged. Only distribution        │
    │   among customers changed.                                                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Interbank Transfer Processing

A transfer between banks requires coordination between two banks' ledgers and settlement through the central bank.

How it works: Bank A sends payment instruction (via SWIFT or other system). Bank A's ledger shows debit to customer and credit to its settlement account at central bank. Bank B's ledger shows credit to its customer and debit to its settlement account. The central bank transfers reserves between the two banks' settlement accounts.

```
INTERBANK TRANSFER PROCESSING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER AT BANK A TRANSFERS $1000 TO CUSTOMER AT BANK B                 │
    │                                                                             │
    │   STEP 1: Bank A processes the outgoing transfer                          │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A Ledger:                                                     │   │
    │   │  ├── Customer A Deposit (Liability): -$1,000 (Debit)                │   │
    │   │  └── Due to Bank B (Liability): +$1,000 (Credit)                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 2: Bank A sends payment message to Bank B (via SWIFT or RTGS)      │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 3: Central bank settles between banks                              │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Central Bank Ledger (RTGS):                                         │   │
    │   │  ├── Bank A Reserve Account: -$1,000 (Debit)                        │   │
    │   │  └── Bank B Reserve Account: +$1,000 (Credit)                       │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 4: Bank B processes incoming transfer                              │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank B Ledger:                                                     │   │
    │   │  ├── Due to Bank A (Liability): -$1,000 (Debit)                     │   │
    │   │  └── Customer B Deposit (Liability): +$1,000 (Credit)               │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Final Result: Money moved from Customer A to Customer B. Bank A's      │
    │   reserves decreased by $1000. Bank B's reserves increased by $1000.      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Bank Money vs Central Bank Money

### The Two Types of Money in Ledgers

Bank ledgers record two fundamentally different types of money: central bank money and commercial bank money.

```
TYPES OF MONEY IN LEDGERS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CENTRAL BANK MONEY (Base money, settlement money)                        │
    │   ├── Recorded on central bank ledger                                       │
    │   ├── Examples: Physical cash, bank reserves at central bank              │
    │   ├── No credit risk (backed by central bank)                              │
    │   └── Used for interbank settlement                                        │
    │                                                                             │
    │   COMMERCIAL BANK MONEY (Deposit money)                                    │
    │   ├── Recorded on commercial bank ledger                                   │
    │   ├── Examples: Checking accounts, savings accounts                        │
    │   ├── Credit risk exists (bank could fail)                                 │
    │   └── Used for everyday transactions                                       │
    │                                                                             │
    │                                                                             │
    │   RELATIONSHIP:                                                            │
    │                                                                             │
    │   Commercial bank money is a claim on central bank money.                 │
    │   A $100 deposit at Bank A is a promise to pay $100 in central bank       │
    │   money on demand.                                                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Ledger Hierarchy

```
LEDGER HIERARCHY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   LEVEL 1: CENTRAL BANK LEDGER                                             │
    │   (Single ledger for entire economy)                                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                    │ Balance                                │   │
    │   │  ───────────────────────────│────────────────────────────────────────│   │
    │   │  Bank A Reserve Account     │ $100,000,000                           │   │
    │   │  Bank B Reserve Account     │ $75,000,000                            │   │
    │   │  Bank C Reserve Account     │ $50,000,000                            │   │
    │   │  Government Account         │ $25,000,000                            │   │
    │   │  Currency in Circulation    │ $200,000,000 (liability)               │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        │ Banks hold reserves at central bank                              │
    │        ▼                                                                   │
    │   LEVEL 2: COMMERCIAL BANK LEDGERS                                         │
    │   (Many ledgers, one per bank)                                            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A Ledger                                                       │   │
    │   │  ├── Customer 1 Deposit: $10,000                                     │   │
    │   │  ├── Customer 2 Deposit: $25,000                                     │   │
    │   │  ├── Loan to Business: $500,000                                      │   │
    │   │  └── Reserve at Central Bank: $100,000,000 (asset)                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        │ Customers hold deposits at commercial banks                     │
    │        ▼                                                                   │
    │   LEVEL 3: CUSTOMER RECORDS                                               │
    │   (Individual tracking, not a ledger)                                     │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Customer 1: $10,000 claim on Bank A                                 │   │
    │   │  Customer 2: $25,000 claim on Bank A                                 │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Money Creation Through Ledgers

### How Lending Creates New Money

When a bank makes a loan, it creates a new deposit in the borrower's account. This creates new commercial bank money that did not exist before.

How it works: The bank does not lend existing deposits. It creates a new deposit liability for the borrower and a new loan asset for itself. The borrower's deposit is new money. This is the fundamental money creation mechanism of fractional reserve banking.

```
LEDGER-BASED MONEY CREATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BEFORE LOAN:                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                   │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Customer Deposits: $100,000  │   │   │
    │   │  │ Loans: $0                   ││ │                             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply = $100,000 (Customer deposits)                             │
    │                                                                             │
    │                                                                             │
    │   BANK MAKES $20,000 LOAN:                                                │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                   │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Customer Deposits: $120,000  │   │   │
    │   │  │ Loans: $20,000 (new)        ││ │                             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply = $120,000 (Customer deposits increased by $20,000)        │
    │                                                                             │
    │   Key insight: New money was created. No existing deposit was used.      │
    │   The bank created a deposit (liability) and a loan (asset)               │
    │   simultaneously.                                                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Money Destruction Through Loan Repayment

When a loan is repaid, the opposite happens: the deposit is debited, and the loan asset is reduced. Money is destroyed.

How it works: The borrower pays from their deposit. The bank reduces both the deposit liability and the loan asset. The deposit disappears from the money supply. Loan repayment is the primary mechanism for money destruction.

```
LOAN REPAYMENT MONEY DESTRUCTION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BEFORE REPAYMENT:                                                        │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                   │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Customer Deposits: $120,000  │   │   │
    │   │  │ Loans: $20,000              ││ │                             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply = $120,000                                                  │
    │                                                                             │
    │                                                                             │
    │   CUSTOMER REPAYS $5,000 OF LOAN:                                          │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                   │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Customer Deposits: $115,000  │   │   │
    │   │  │ Loans: $15,000              ││ │                             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply = $115,000 ($5,000 destroyed)                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Ledger Reconciliation

### Daily Reconciliation Process

Banks must reconcile their ledgers daily to ensure all entries are correct and the accounting equation balances.

```
DAILY RECONCILIATION PROCESS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STEP 1: SUBSIDIARY LEDGER TOTALS                                         │
    │   ├── Sum all customer deposit balances                                    │
    │   ├── Sum all loan balances                                                │
    │   ├── Sum all other subsidiary records                                     │
    │   └── Compare to control account balances in general ledger               │
    │                                                                             │
    │   STEP 2: TRANSACTION LOG REVIEW                                           │
    │   ├── Verify each transaction has equal debits and credits                │
    │   ├── Check for unauthorized or suspicious entries                        │
    │   └── Investigate any unbalanced entries                                   │
    │                                                                             │
    │   STEP 3: CASH RECONCILIATION                                              │
    │   ├── Count physical vault cash                                            │
    │   ├── Compare to vault cash ledger balance                                 │
    │   └── Investigate discrepancies                                            │
    │                                                                             │
    │   STEP 4: CENTRAL BANK RESERVE RECONCILIATION                              │
    │   ├── Compare bank's reserve ledger to central bank statement             │
    │   ├── Adjust for uncleared checks and floats                              │
    │   └── Report any discrepancies                                             │
    │                                                                             │
    │   STEP 5: GENERAL LEDGER BALANCE                                          │
    │   ├── Verify total assets = total liabilities + equity                    │
    │   ├── Post adjusting entries if needed                                    │
    │   └── Produce daily balance sheet                                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Common Reconciliation Issues

```
RECONCILIATION ISSUES AND RESOLUTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Issue                    │ Cause                    │ Resolution        │
    │   ─────────────────────────│──────────────────────────│───────────────────│
    │   Out of balance           │ Data entry error,         │ Find and correct  │
    │   (Assets ≠ Liabilities    │ missing transaction,      │ erroneous entry   │    │   + Equity)                │ system bug                │                   │
    │   ─────────────────────────│──────────────────────────│───────────────────│
    │   Customer balance         │ Unposted transaction,     │ Post missing      │
    │   discrepancy              │ timing difference         │ transactions,     │
    │                           │                           │ adjust for floats │
    │   ─────────────────────────│──────────────────────────│───────────────────│
    │   Vault cash mismatch      │ Counting error, theft,    │ Recount,          │
    │                           │ unrecorded deposits/      │ investigate,      │
    │                           │ withdrawals               │ adjust ledger     │
    │   ─────────────────────────│──────────────────────────│───────────────────│
    │   Reserve account          │ Uncleared checks,         │ Identify          │
    │   difference               │ timing of settlements     │ outstanding       │
    │                           │                           │ items             │
    │   ─────────────────────────│──────────────────────────│───────────────────│
    │   Duplicate transaction    │ System error,             │ Reverse one       │
    │                           │ manual double-entry       │ entry             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Evolution of Bank Ledgers

### Physical Ledgers (Pre-1960s)

Before computerization, bank ledgers were physical books. Each account had a page or card. Transactions were written by hand.

How it worked: Clerks manually recorded each transaction in the customer's ledger card. Daily totals were calculated by hand. End-of-day balancing required dozens of clerks adding columns. Errors were common and required extensive manual searching.

### Mainframe Ledgers (1960s-1990s)

Banks computerized their ledgers using mainframe computers. Transactions were entered via terminals and processed in batch overnight.

How it worked: Daily transactions were keypunched onto cards or magnetic tape. Overnight batch processing updated all accounts. Customers saw next-day balances. Core banking systems from IBM, Unisys dominated.

### Online Real-Time Ledgers (1990s-2010s)

Real-time processing allowed immediate transaction posting. Customers could see current balances instantly.

How it worked: Transactions processed immediately. Database systems (Oracle, DB2, SQL Server) stored ledgers. 24/7 operations replaced overnight batch. ATMs, online banking, and debit cards became possible.

### Distributed Ledger Technology (2010s-present)

Distributed ledger technology (DLT) allows multiple parties to share and synchronize a ledger without a central authority. Each participant has a copy, and consensus mechanisms ensure all copies match.

How it works: Transactions are grouped into blocks. Each block is cryptographically linked to the previous block (blockchain). Multiple nodes validate transactions through consensus (proof of work, proof of stake, or other mechanisms). Once confirmed, transactions are immutable (cannot be changed).

```
DLT VS TRADITIONAL LEDGER

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Feature              │ Traditional Ledger    │ Distributed Ledger       │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Central authority    │ Yes (bank maintains)  │ No (shared among          │
    │                       │                       │ participants)            │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Single point of      │ Yes                   │ No                        │
    │   failure              │                       │                           │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Trust model          │ Trust in central      │ Cryptographic proof +    │
    │                       │ party                 │ consensus                 │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Transaction speed    │ Very fast (internal)  │ Slower (consensus delay) │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Immutability         │ Can be changed        │ Extremely difficult      │
    │                       │ (administrator)       │ to alter                  │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Transparency         │ Private (bank only)   │ Public or permissioned   │
    │   ─────────────────────│───────────────────────│──────────────────────────│
    │   Energy efficiency    │ High                   │ Low (proof of work) or   │
    │                       │                        │ moderate (other          │
    │                       │                        │ consensus)               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
LEDGER FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Accounting Equation: Assets = Liabilities + Equity                       │
    │                                                                             │
    │   Debits = Credits (for every transaction)                                 │
    │                                                                             │
    │   Control Account Balance = Sum of Subsidiary Ledger Balances              │
    │                                                                             │
    │   Customer Available Balance = Ledger Balance - Holds - Uncleared Items    │
    │                                                                             │
    │   Bank Reserve Balance = Deposits at Central Bank - Borrowings             │
    │                                                                             │
    │   Money Supply (M1) = Currency + Demand Deposits                          │
    │                                                                             │
    │   Money Creation (per loan) = ΔDeposits = ΔLoans                           │
    │                                                                             │
    │   Money Destruction (per repayment) = ΔDeposits = -ΔLoans                  │
    │                                                                             │
    │   Net Interest Income = Interest Received - Interest Paid                  │
    │                                                                             │
    │   Bank Capital Ratio = Equity / Risk-Weighted Assets                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Bank ledger is the official record of all financial transactions and account balances.

2. Fundamental identity: Assets = Liabilities + Equity. Ledger must always balance.

3. Double-entry bookkeeping: Every transaction has equal debits and credits.

4. Debits increase assets/expenses. Credits increase liabilities/equity/revenue.

5. General ledger contains summary control accounts. Subsidiary ledgers contain detailed individual records.

6. Customer deposits are liabilities of the bank, not assets. The bank owes this money to customers.

7. Internal transfers: Debit one customer account, credit another. Total liabilities unchanged.

8. Interbank transfers require settlement through central bank reserve accounts.

9. Central bank money: recorded on central bank ledger. No credit risk.

10. Commercial bank money: recorded on commercial bank ledger. Credit risk exists.

11. Money creation: Bank makes loan → creates new deposit liability → new money exists.

12. Money destruction: Loan repayment → deposit debited → money disappears.

13. Daily reconciliation ensures ledger accuracy and detects errors or fraud.

14. Physical ledgers (pre-1960s): handwritten books, manual calculation.

15. Mainframe ledgers (1960s-1990s): computerized, batch processing, overnight updates.

16. Online real-time ledgers (1990s-2010s): immediate posting, 24/7 availability.

17. Distributed ledger technology (2010s-present): shared ledger, no central authority, cryptographic verification.

18. DLT advantages: no single point of failure, immutability, transparency.

19. DLT disadvantages: slower, energy-intensive (proof of work), scalability challenges.

20. Bank ledgers are the foundation of the monetary system. Every dollar in existence is recorded somewhere on a ledger.

*This documentation belongs to https://github.com/InterCentury*