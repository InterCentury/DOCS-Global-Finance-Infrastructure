# 04 - Commercial Banks

## Documentation Overview

Commercial banks are financial institutions that accept deposits from the public, provide checking and savings accounts, and make loans to individuals and businesses. They are the primary creators of broad money (M1/M2) through fractional reserve banking and serve as the main interface between the financial system and the real economy. This document covers the functions, balance sheet structure, operations, risks, and regulation of commercial banks.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the core functions of commercial banks                         │
    │   Learn the balance sheet structure and key accounts                        │
    │   Study deposit taking and lending operations                               │
    │   Analyze money creation through lending                                    │
    │   Examine the role of banks in payment processing                           │
    │   Understand bank risks (credit, liquidity, market, operational)            │
    │   Learn capital requirements and prudential regulation                      │
    │   Study bank business models and revenue sources                            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Core Functions

### What is a Commercial Bank

A commercial bank is a financial intermediary that accepts deposits from the public and uses those funds to make loans. Unlike investment banks, commercial banks focus on deposit taking and lending to households and businesses.

How it works: Customers deposit money into checking and savings accounts. The bank holds a fraction of these deposits as reserves (vault cash and central bank deposits) and lends the remainder to borrowers. The bank earns interest on loans and pays interest on deposits, profiting from the spread. Deposits are liabilities of the bank (money owed to customers), while loans are assets (money owed to the bank).

```
COMMERCIAL BANK CORE FUNCTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │                       COMMERCIAL BANK                               │   │
    │   │                             │                                       │   │
    │   │         ┌───────────────────┼───────────────────┐                   │   │
    │   │         │                   │                   │                   │   │
    │   │         ▼                   ▼                   ▼                   │   │
    │   │   ┌───────────┐       ┌───────────┐       ┌───────────┐             │   │
    │   │   │ Deposit   │       │ Lending   │       │ Payment   │             │   │
    │   │   │ Taking    │       │           │       │ Processing│             │   │
    │   │   └─────┬─────┘       └─────┬─────┘       └─────┬─────┘             │   │
    │   │         │                   │                   │                   │   │
    │   │         └───────────────────┼───────────────────┘                   │   │
    │   │                             │                                       │   │
    │   │         ┌───────────────────┼───────────────────┐                   │   │
    │   │         │                   │                   │                   │   │
    │   │         ▼                   ▼                   ▼                   │   │
    │   │   ┌──────────────┐   ┌──────────────┐    ┌──────────────┐           │   │
    │   │   │Maturity      │   │Risk          │    │Liquidity     │           │   │
    │   │   │Transformation│   │Transformation│    │Transformation│           │   │
    │   │   └──────────────┘   └──────────────┘    └──────────────┘           │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   FUNCTION DETAILS:                                                         │
    │                                                                             │
    │   1. Deposit Taking: Accepts funds from depositors in exchange for          │
    │      interest and transactional services. Creates bank liabilities.         │
    │                                                                             │
    │   2. Lending: Provides loans to households (mortgages, auto, personal)      │
    │      and businesses (working capital, expansion, equipment). Creates        │
    │      bank assets and new deposits (money creation).                         │
    │                                                                             │
    │   3. Payment Processing: Facilitates transfers between accounts,            │
    │      issues checks and debit cards, processes direct deposits.              │
    │                                                                             │
    │   4. Maturity Transformation: Borrows short (deposits can be withdrawn      │
    │      anytime) and lends long (mortgages for 30 years).                      │
    │                                                                             │
    │   5. Risk Transformation: Takes on credit risk from borrowers, provides     │
    │      depositors with safe, insured claims.                                  │
    │                                                                             │
    │   6. Liquidity Transformation: Converts illiquid loans into liquid          │
    │      deposits that can be withdrawn on demand.                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Banks vs Other Financial Institutions

```
BANK VS NON-BANK COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Feature              │ Commercial Bank    │ Credit Union │ Shadow Bank    │
    │   ─────────────────────│────────────────────│──────────────│─────────────── │
    │   Ownership            │ Shareholder-owned  │ Member-owned │ Investor-owned │
    │   ─────────────────────│────────────────────│──────────────│─────────────── │
    │   Deposit insurance    │ Yes (FDIC, etc.)   │ Yes          │ No             │
    │   ─────────────────────│────────────────────│──────────────│─────────────── │
    │   Access to central    │ Yes (discount      │ Limited      │ No             │
    │   bank liquidity       │ window)            │              │                │
    │   ─────────────────────│────────────────────│──────────────│─────────────── │
    │   Money creation       │ Yes (through       │ No (must     │ No             │
    │   power                │ lending)           │ hold 100%    │                │
    │                        │                    │ reserves?)   │                │
    │   ─────────────────────│────────────────────│──────────────│─────────────── │
    │   Primary regulator    │ Central bank /     │ NCUA / state │ SEC /          │
    │                        │ banking agency     │              │ CFTC           │
    │   ─────────────────────│────────────────────│──────────────│─────────────── │
    │   Examples             │ JPMorgan, Chase,   │ Navy Federal,│ Blackstone,    │
    │                        │ Bank of America    │ State Farm   │ Bridgewater    │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Bank Balance Sheet

### Structure of Commercial Bank Balance Sheet

The bank balance sheet shows assets (what the bank owns) on the left and liabilities plus equity (what the bank owes) on the right.

```
COMMERCIAL BANK BALANCE SHEET

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ASSETS                                    LIABILITIES                     │
    │   ───────────────────────────               ───────────────────────────     │
    │                                             │                               │
    │   ┌─────────────────────────────┐           ┌─────────────────────────────┐ │
    │   │ Cash and Reserves           │           │ Deposits                    │ │
    │   │ ├── Vault cash              │           │ ├── Demand deposits         │ │
    │   │ └── Reserves at central bank│           │ │   (checking)              │ │
    │   └─────────────────────────────┘           │ ├── Savings deposits        │ │
    │                                             │ └── Time deposits (CDs)     │ │
    │   ┌─────────────────────────────┐           └─────────────────────────────┘ │
    │   │ Securities                  │           ┌─────────────────────────────┐ │
    │   │ ├── Treasury bonds          │           │ Borrowings                  │ │
    │   │ ├── Agency securities       │           │ ├── Federal funds purchased │ │
    │   │ └── Municipal bonds         │           │ ├── Discount window loans   │ │
    │   └─────────────────────────────┘           │ └── Other borrowings        │ │
    │                                             └─────────────────────────────┘ │
    │   ┌─────────────────────────────┐           ┌─────────────────────────────┐ │
    │   │ Loans (Gross)               │           │ Other Liabilities           │ │
    │   │ ├── Commercial loans        │           │ └── Accrued expenses, etc.  │ │
    │   │ ├── Real estate loans       │           └─────────────────────────────┘ │
    │   │ ├── Consumer loans          │                                           │
    │   │ └── Other loans             │           ┌─────────────────────────────┐ │
    │   └─────────────────────────────┘           │ EQUITY                      │ │
    │                                             │ ├── Share capital           │ │
    │   ┌─────────────────────────────┐           │ ├── Retained earnings       │ │
    │   │ Loan Loss Reserve           │           │ └── Other equity accounts   │ │
    │   │ (Contra-asset, negative)    │           └─────────────────────────────┘ │
    │   └─────────────────────────────┘                                           │
    │   ┌─────────────────────────────┐                                           │
    │   │ Other Assets                │                                           │
    │   │ ├── Bank premises           │                                           │
    │   │ └── Other real estate owned │                                           │
    │   └─────────────────────────────┘                                           │
    │                                                                             │
    │   ───────────────────────────               ───────────────────────────     │
    │   TOTAL ASSETS                 =            TOTAL LIABILITIES + EQUITY      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Key Balance Sheet Accounts

```
KEY ACCOUNTS EXPLANATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   ACCOUNT                    │ TYPE      │ DESCRIPTION                      │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Vault Cash                 │ Asset     │ Physical currency held in        │
    │                              │           │ bank premises and ATMs           │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Reserves at Central Bank   │ Asset     │ Digital account balance at       │
    │                              │           │ central bank for settlement      │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Securities                 │ Asset     │ Government and agency bonds      │
    │                              │           │ held for liquidity and yield     │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Loans (Gross)              │ Asset     │ Total value of all loans made    │
    │                              │           │ (before reserves for losses)     │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Loan Loss Reserve          │ Contra-   │ Estimated losses on loans.       │
    │   (Allowance)                │ asset     │ Reduces reported loan value.     │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Loans (Net)                │ Asset     │ Gross loans minus loan loss      │
    │                              │           │ reserve. Carrying value.         │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Demand Deposits            │ Liability │ Checking accounts. Payable       │
    │   (Checking)                 │           │ on demand. No interest (usually) │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Savings Deposits           │ Liability │ Interest-bearing accounts.       │
    │                              │           │ Limited transactions.            │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Time Deposits (CDs)        │ Liability │ Fixed-term deposits. Penalty     │
    │                              │           │ for early withdrawal.            │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Borrowings                 │ Liability │ Funds borrowed from other        │
    │                              │           │ banks or central bank.           │
    │   ───────────────────────────│───────────│───────────────────────────────── │
    │   Equity (Capital)           │ Equity    │ Shareholder investment +         │
    │                              │           │ retained earnings. Loss-         │
    │                              │           │ absorbing buffer.                │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Deposit Taking

### Types of Deposits

Banks offer various deposit products to attract funds from different customer segments.

```
DEPOSIT TYPES COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Deposit Type     │ Interest  │ Liquidity    │ Insurance  │ Primary Users  │
    │   ─────────────────│───────────│──────────────│────────────│─────────────── │
    │   Demand Deposit   │ None or   │ Immediate    │ Yes        │ Households,    │
    │   (Checking)       │ very low  │ (unlimited   │            │ businesses     │
    │                    │           │ withdrawals) │            │                │
    │   ─────────────────│───────────│──────────────│────────────│─────────────── │
    │   NOW Account      │ Low       │ Immediate    │ Yes        │ Households     │
    │   (Interest-       │           │ (checks)     │            │                │
    │    checking)       │           │              │            │                │
    │   ─────────────────│───────────│──────────────│────────────│─────────────── │
    │   Savings Account  │ Low to    │ Immediate    │ Yes        │ Households     │
    │                    │ moderate  │ (limited     │            │                │
    │                    │           │ transfers)   │            │                │
    │   ─────────────────│───────────│──────────────│────────────│─────────────── │
    │   Money Market     │ Moderate  │ Limited      │ Yes        │ Households,    │
    │   Deposit Account  │           │ checks       │            │ small business │
    │   ─────────────────│───────────│──────────────│────────────│─────────────── │
    │   Certificate of   │ Higher    │ Low (penalty │ Yes        │ Savers,        │
    │   Deposit (CD)     │ (fixed    │ for early    │            │ retirees       │
    │                    │ term)     │ withdrawal)  │            │                │
    │   ─────────────────│───────────│──────────────│────────────│─────────────── │
    │   Jumbo CD         │ Highest   │ Low (penalty │ Partial    │ Institutional, │
    │   (>$100k)         │           │ for early    │ (over      │ corporations   │
    │                    │           │ withdrawal)  │ limit)     │                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### How Deposit Taking Works

When a customer deposits money, the bank's balance sheet expands. The bank gains an asset (cash or reserves) and incurs a liability (deposit obligation).

How it works: Customer brings $1000 cash to bank. Bank adds $1000 to vault cash (asset) and credits customer's deposit account (liability). The bank now owes the customer $1000. The customer can withdraw, write checks, or transfer this money at any time.

```
DEPOSIT PROCESSING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER DEPOSITS $1000 CASH                                              │
    │                                                                             │
    │   BEFORE DEPOSIT:                                                           │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                  │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Vault Cash: $10,000         ││ │ Customer Deposits: $100,000 │   │   │
    │   │  │ Loans: $500,000             ││ │ Equity: $50,000             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   AFTER DEPOSIT:                                                            │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                  │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Vault Cash: $11,000 (+$1k)  ││ │ Customer Deposits: $101,000 │   │   │
    │   │  │ Loans: $500,000             ││ │   (+$1k)                    │   │   │
    │   │  └─────────────────────────────┘│ │ Equity: $50,000             │   │   │
    │   │                                 │ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Key insight: Both sides of balance sheet increased by $1000.              │
    │   Bank now has more cash (asset) and more deposit liability.                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Lending and Money Creation

### How Banks Create Money

When a bank makes a loan, it creates a new deposit in the borrower's account. This creates new money that did not exist before.

How it works: Bank approves a $10,000 loan to a customer. The bank adds a $10,000 loan asset to its balance sheet. It also credits the customer's deposit account with $10,000 (liability). No existing deposit was used. New money is created. The customer can now spend this new money.

```
MONEY CREATION THROUGH LENDING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BEFORE LOAN:                                                              │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                  │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Deposits: $100,000          │   │   │
    │   │  │ Loans: $0                   ││ │ Equity: $10,000             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply (deposits) = $100,000                                        │
    │                                                                             │
    │                                                                             │
    │   BANK MAKES $20,000 LOAN:                                                  │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                  │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Deposits: $120,000          │   │   │
    │   │  │ Loans: $20,000 (new)        ││ │   (+$20,000)                │   │   │
    │   │  └─────────────────────────────┘│ │ Equity: $10,000             │   │   │
    │   │                                 │ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply (deposits) = $120,000 (+$20,000 created)                     │
    │                                                                             │
    │   Key insight: The loan created a new deposit. No existing deposit          │
    │   was used. Money was created from nothing.                                 │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Types of Loans

Banks offer various loan products for different purposes and risk profiles.

```
LOAN TYPES COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Loan Type        │ Purpose              │ Term       │ Collateral       │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Residential      │ Home purchase        │ 15-30 years│ Property         │
    │   Mortgage         │                      │            │                  │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Commercial Real  │ Office buildings,    │ 5-20 years │ Property         │
    │   Estate (CRE)     │ retail, industrial   │            │                  │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Commercial and   │ Working capital,     │ 1-7 years  │ Business assets, │
    │   Industrial (C&I) │ equipment, expansion │            │ personal guaranty│
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Auto Loan        │ Vehicle purchase     │ 3-7 years  │ Vehicle          │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Credit Card      │ Revolving spending   │ Revolving  │ Unsecured        │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Personal Loan    │ Debt consolidation,  │ 1-5 years  │ Unsecured        │
    │                    │ medical, etc.        │            │                  │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Small Business   │ Startup, expansion   │ 5-10 years │ Business assets, │
    │   Administration   │ (SBA guaranteed)     │            │ SBA guarantee    │
    │   (SBA)            │                      │            │                  │
    │   ─────────────────│──────────────────────│────────────│──────────────────│
    │   Overdraft        │ Temporary negative   │ Demand     │ Deposits         │
    │   Protection       │ balance coverage     │            │                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Loan Underwriting Process

Banks evaluate loan applications using the "Five C's of Credit" framework.

```
FIVE C'S OF CREDIT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   1. CHARACTER                                                            │
    │      ├── Borrower's credit history and payment record                     │
    │      ├── Credit score (FICO, VantageScore)                                │
    │      ├── Past bankruptcies or defaults                                    │
    │      └── Stability of employment/residence                               │
    │                                                                             │
    │   2. CAPACITY                                                             │
    │      ├── Ability to repay from income                                     │
    │      ├── Debt-to-income ratio (DTI)                                       │
    │      ├── Cash flow analysis                                               │
    │      └── Employment history and income stability                          │
    │                                                                             │
    │   3. CAPITAL                                                              │
    │      ├── Down payment or equity contribution                              │
    │      ├── Borrower's net worth                                             │
    │      ├── Liquid assets available                                          │
    │      └── Skin in the game                                                │
    │                                                                             │
    │   4. COLLATERAL                                                           │
    │      ├── Assets pledged to secure loan                                    │
    │      ├── Loan-to-value ratio (LTV)                                        │
    │      ├── Quality and liquidity of collateral                              │
    │      └── Appraised value                                                 │
    │                                                                             │
    │   5. CONDITIONS                                                           │
    │      ├── Purpose of loan                                                  │
    │      ├── Economic environment                                             │
    │      ├── Industry conditions                                              │
    │      ├── Interest rate environment                                        │
    │      └── Loan terms and covenants                                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Payment Processing

### Role in Payment System

Banks are the primary intermediaries for payments. They maintain customer accounts and facilitate fund transfers.

How it works: When a customer writes a check or uses a debit card, the bank debits the customer's account and credits the merchant's account (if same bank) or sends payment instructions to another bank. Banks settle interbank payments through their reserve accounts at the central bank.

```
PAYMENT PROCESSING FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER PAYS MERCHANT $100 WITH DEBIT CARD                             │
    │                                                                             │
    │   STEP 1: Merchant submits transaction to acquiring bank                  │
    │                                                                             │
    │   STEP 2: Acquiring bank routes to card network (Visa, Mastercard)        │
    │                                                                             │
    │   STEP 3: Card network routes to issuing bank (customer's bank)           │
    │                                                                             │
    │   STEP 4: Issuing bank verifies funds and authorizes                      │
    │                                                                             │
    │   STEP 5: Funds move from issuing bank to acquiring bank                  │
    │                                                                             │
    │   STEP 6: Acquiring bank credits merchant's account                       │
    │                                                                             │
    │                                                                             │
    │   LEDGER ENTRIES:                                                          │
    │                                                                             │
    │   Issuing Bank:                                                           │
    │   ├── Debit: Customer Deposit (liability) -$100                          │
    │   └── Credit: Due to Acquiring Bank (liability) +$100                    │
    │                                                                             │
    │   Acquiring Bank:                                                         │
    │   ├── Debit: Due from Issuing Bank (asset) +$100                         │
    │   └── Credit: Merchant Deposit (liability) +$100                         │
    │                                                                             │
    │   Central Bank Settlement (end of day or real-time):                      │
    │   ├── Debit: Issuing Bank Reserve Account -$100                          │
    │   └── Credit: Acquiring Bank Reserve Account +$100                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Check Clearing

Checks are paper instruments that instruct a bank to transfer funds from the check writer's account to the payee's account.

How it works: Payee deposits check at their bank. Payee's bank sends check to check writer's bank (through clearing house or directly). Check writer's bank verifies signature and funds, then debits the account. Funds are transferred between banks through reserve accounts.

## Bank Revenue and Profitability

### Sources of Revenue

Banks earn revenue primarily from interest on loans and fees from services.

```
BANK REVENUE SOURCES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   REVENUE TYPE              │ SOURCE                     │ TYPICAL SHARE   │
    │   ──────────────────────────│────────────────────────────│─────────────────│
    │   Net Interest Income       │ Interest on loans minus    │ 60-70%          │
    │   (NII)                    │ interest on deposits       │                 │
    │   ──────────────────────────│────────────────────────────│─────────────────│
    │   Non-Interest Income       │                            │ 30-40%          │
    │   ├── Deposit fees          │ Overdraft, monthly         │                 │
    │   │                        │ maintenance, ATM           │                 │
    │   ├── Credit card fees      │ Annual fees, late fees,    │                 │
    │   │                        │ interchange                │                 │
    │   ├── Mortgage fees         │ Origination, processing,   │                 │
    │   │                        │ servicing                  │                 │
    │   ├── Wealth management     │ Advisory fees, asset       │                 │
    │   │                        │ management fees            │                 │
    │   ├── Investment banking    │ Underwriting, advisory     │ (large banks    │
    │   │                        │                            │  only)          │
    │   └── Trading revenue       │ Market making, proprietary │ (large banks    │
    │                            │ trading                    │  only)          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Net Interest Margin (NIM)

Net interest margin is the difference between interest earned on assets and interest paid on liabilities, expressed as a percentage of earning assets.

How it works: Bank earns 5% on loans and pays 1% on deposits. The 4% spread is the gross interest margin. After accounting for non-performing loans and other costs, the net interest margin might be 3.5%. NIM is a key profitability metric.

```
NET INTEREST MARGIN CALCULATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FORMULA: NIM = (Interest Income - Interest Expense) / Earning Assets     │
    │                                                                             │
    │   EXAMPLE:                                                                 │
    │                                                                             │
    │   Interest Income:                                                         │
    │   ├── Loan interest: $500 million                                         │
    │   └── Securities interest: $50 million                                    │
    │   Total Interest Income: $550 million                                     │
    │                                                                             │
    │   Interest Expense:                                                        │
    │   ├── Deposit interest: $100 million                                      │
    │   └── Borrowing interest: $50 million                                     │
    │   Total Interest Expense: $150 million                                    │
    │                                                                             │
    │   Net Interest Income: $550M - $150M = $400 million                       │
    │                                                                             │
    │   Earning Assets: $10 billion                                             │
    │                                                                             │
    │   NIM = $400M / $10,000M = 4.00%                                          │
    │                                                                             │
    │   Industry average NIM: 3.0-4.5% (varies by bank size and business model)│
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Bank Risks

### Credit Risk

Credit risk is the risk that a borrower will default on a loan, causing the bank to lose principal and interest.

How it works: Bank lends $100,000 to a business. Business fails and cannot repay. Bank writes off the loan as a loss. Loan loss reserves are set aside to absorb expected losses. Unexpected losses are absorbed by bank capital.

```
CREDIT RISK MANAGEMENT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MITIGATION TOOLS:                                                        │
    │                                                                             │
    │   1. Underwriting Standards                                                │
    │      ├── Credit scoring and analysis                                       │
    │      ├── Debt-to-income limits                                            │
    │      └── Loan-to-value limits                                             │
    │                                                                             │
    │   2. Collateral                                                            │
    │      ├── Secured by assets (property, equipment, deposits)                │
    │      ├── Lien on collateral                                               │
    │      └── Foreclosure or repossession rights                               │
    │                                                                             │
    │   3. Diversification                                                       │
    │      ├── Across borrowers (not concentrated in one customer)              │
    │      ├── Across industries (not concentrated in oil, real estate, etc.)   │
    │      └── Across geographies                                                │
    │                                                                             │
    │   4. Loan Loss Reserves (Allowance)                                        │
    │      ├── Provision for expected losses                                    │
    │      ├── Based on historical default rates                                │
    │      ├── Adjusted for economic conditions                                 │
    │      └── CECL (Current Expected Credit Losses) standard                   │
    │                                                                             │
    │   5. Capital                                                               │
    │      ├── Equity absorbs unexpected losses                                 │
    │      ├── Higher capital = greater loss absorption                         │
    │      └── Regulatory minimums (4.5% CET1)                                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Liquidity Risk

Liquidity risk is the risk that a bank cannot meet its short-term obligations (deposit withdrawals, payment demands) without incurring unacceptable losses.

How it works: Bank has $100 million in deposits that can be withdrawn anytime. It has only $10 million in cash and reserves. Under normal conditions, only 5-10% of depositors withdraw at once. During a panic, withdrawals could exceed reserves. The bank must borrow or sell assets quickly, potentially at fire-sale prices.

```
LIQUIDITY RISK MANAGEMENT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MITIGATION TOOLS:                                                        │
    │                                                                             │
    │   1. Liquid Asset Buffer                                                   │
    │      ├── Cash and central bank reserves                                   │
    │      ├── Treasury securities (highly liquid)                              │
    │      ├── Agency securities                                                 │
    │      └── High-quality corporate bonds                                     │
    │                                                                             │
    │   2. Liquidity Coverage Ratio (LCR) - Basel III                           │
    │      ├── High-quality liquid assets (HQLA) / Net cash outflows (30 days)  │
    │      ├── Minimum 100%                                                     │
    │      └── Ensures bank can survive 30-day stress scenario                  │
    │                                                                             │
    │   3. Net Stable Funding Ratio (NSFR) - Basel III                          │
    │      ├── Available stable funding / Required stable funding               │
    │      ├── Minimum 100%                                                     │
    │      └── Encourages long-term funding for long-term assets                │
    │                                                                             │
    │   4. Contingency Funding Plan                                              │
    │      ├── Identifies liquidity stress triggers                            │
    │      ├── Lists available funding sources                                  │
    │      └── Specifies actions during crisis                                  │
    │                                                                             │
    │   5. Access to Central Bank                                                │
    │      ├── Discount window borrowing                                        │
    │      ├── Standing lending facilities                                      │
    │      └── Emergency liquidity assistance                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Market Risk

Market risk is the risk of losses from changes in market prices: interest rates, exchange rates, equity prices, commodity prices.

How it works: Bank holds $1 billion in long-term fixed-rate bonds. Interest rates rise by 1%. Bond prices fall by approximately 10% (duration effect). Bank loses $100 million in market value. If the bonds are held for investment (not trading), the loss may not be realized but still affects capital.

```
INTEREST RATE RISK EXAMPLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BANK BALANCE SHEET (Simplified)                                          │
    │                                                                             │
    │   Assets (Rate-sensitive)              Liabilities (Rate-sensitive)        │
    │   ├── Floating-rate loans: $500M       ├── Floating-rate deposits: $300M   │
    │   ├── Fixed-rate loans: $800M          ├── Fixed-rate deposits: $600M      │
    │   └── Securities: $200M                └── Equity: $200M                   │
    │                                                                             │
    │   GAP ANALYSIS:                                                            │
    │                                                                             │
    │   Rate-Sensitive Assets (RSA) = $500M (floating loans)                    │
    │   Rate-Sensitive Liabilities (RSL) = $300M (floating deposits)            │
    │   Gap = RSA - RSL = +$200M                                                │
    │                                                                             │
    │   If rates rise 1%: Net interest income increases ~$200M × 1% = $2M      │
    │   If rates fall 1%: Net interest income decreases ~$2M                    │
    │                                                                             │
    │   DURATION GAP (Fixed-rate positions):                                     │
    │   Fixed-rate assets ($800M + $200M = $1B) with duration 5 years           │
    │   Fixed-rate liabilities ($600M) with duration 1 year                     │
    │   Duration gap exposes bank to falling asset values if rates rise         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Operational Risk

Operational risk is the risk of loss from inadequate or failed internal processes, people, systems, or external events.

How it works: A systems failure prevents customers from accessing accounts. A rogue trader exceeds authorized limits and hides losses. An employee embezzles funds. A cyberattack steals customer data. A natural disaster destroys a data center.

```
OPERATIONAL RISK CATEGORIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CATEGORY              │ EXAMPLES                                         │
    │   ──────────────────────│──────────────────────────────────────────────────│
    │   Internal Fraud        │ Employee theft, embezzlement, unauthorized      │
    │                        │ trading, insider trading                         │
    │   ──────────────────────│──────────────────────────────────────────────────│
    │   External Fraud        │ Cyberattacks, check fraud, identity theft,      │
    │                        │ phishing, ransomware                             │
    │   ──────────────────────│──────────────────────────────────────────────────│
    │   Employment Practices  │ Discrimination claims, wrongful termination,   │
    │                        │ workplace safety violations                      │
    │   ──────────────────────│──────────────────────────────────────────────────│
    │   Business Disruption   │ Systems failure, power outage, natural         │
    │                        │ disaster, pandemic                               │
    │   ──────────────────────│──────────────────────────────────────────────────│
    │   Process Management    │ Data entry errors, document processing         │
    │                        │ failures, model errors                           │
    │   ──────────────────────│──────────────────────────────────────────────────│
    │   Technology Failure    │ Software bugs, hardware failure, network       │
    │                        │ outage, data corruption                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Capital Requirements

### Basel Framework

The Basel framework (Basel I, II, III) sets international standards for bank capital, liquidity, and risk management.

```
BASEL CAPITAL REQUIREMENTS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CAPITAL TIERS:                                                           │
    │                                                                             │
    │   Common Equity Tier 1 (CET1) - Highest quality                           │
    │   ├── Common shares (stock)                                               │
    │   ├── Retained earnings                                                   │
    │   ├── Other comprehensive income                                          │
    │   └── Minimum requirement: 4.5% of risk-weighted assets (RWA)            │
    │                                                                             │
    │   Additional Tier 1 (AT1)                                                 │
    │   ├── Preferred stock (non-cumulative)                                    │
    │   ├── Contingent convertible bonds (CoCos)                               │
    │   └── Minimum requirement: 1.5% of RWA                                   │
    │                                                                             │
    │   Tier 2 Capital                                                          │
    │   ├── Subordinated debt                                                   │
    │   ├── Loan loss reserves (limited)                                        │
    │   └── Minimum requirement: 2.0% of RWA                                    │
    │                                                                             │
    │                                                                             │
    │   TOTAL CAPITAL REQUIREMENTS:                                             │
    │                                                                             │
    │   CET1: 4.5% + CCyB (0-2.5%) + G-SIB surcharge (1-3.5%) = typically 7-10%│
    │   Tier 1: 6.0% + buffers                                                   │
    │   Total Capital: 8.0% + buffers                                           │
    │                                                                             │
    │   Plus Capital Conservation Buffer: 2.5% (CET1)                          │
    │   Plus Countercyclical Buffer: 0-2.5% (national discretion)              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Risk-Weighted Assets

Different assets have different risk weights. A $100 loan to a corporation has higher risk weight than a $100 Treasury bond.

```
RISK WEIGHTS (Simplified Basel III)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Asset Type                           │ Risk Weight (%)                   │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Cash and central bank reserves       │ 0%                                │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Government bonds (OECD)              │ 0%                                │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Claims on other banks                │ 20%                               │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Residential mortgages                │ 35%                               │
    │   (conservative LTV)                   │                                   │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Corporate loans (investment grade)   │ 50-100%                           │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Corporate loans (non-investment      │ 100% (or higher)                  │
    │   grade)                               │                                   │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Unsecured consumer loans              │ 100%                              │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Equity investments                    │ 300-400%                          │
    │   ─────────────────────────────────────│───────────────────────────────────│
    │   Past due loans (>90 days)            │ 150%                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Bank Regulation and Supervision

### Regulatory Framework

Banks are heavily regulated to ensure safety, soundness, and consumer protection.

```
REGULATORY BODIES (US Example)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   REGULATOR                    │ PRIMARY RESPONSIBILITY                    │
    │   ─────────────────────────────│────────────────────────────────────────────│
    │   Federal Reserve (Fed)        │ Bank holding companies, state member      │
    │                               │ banks, monetary policy, lender of last     │
    │                               │ resort                                     │
    │   ─────────────────────────────│────────────────────────────────────────────│
    │   Office of the Comptroller    │ National banks and federal savings        │
    │   of the Currency (OCC)        │ associations                              │
    │   ─────────────────────────────│────────────────────────────────────────────│
    │   Federal Deposit Insurance    │ State non-member banks, deposit           │
    │   Corporation (FDIC)           │ insurance (up to $250,000)                │
    │   ─────────────────────────────│────────────────────────────────────────────│
    │   Consumer Financial           │ Consumer protection, fair lending         │
    │   Protection Bureau (CFPB)     │                                           │
    │   ─────────────────────────────│────────────────────────────────────────────│
    │   State Banking Departments    │ State-chartered banks                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Deposit Insurance

Deposit insurance guarantees depositors will be repaid up to a limit if their bank fails. This prevents bank runs.

How it works: FDIC insures deposits up to $250,000 per depositor, per bank, per ownership category. If a bank fails, the FDIC pays depositors directly or arranges a transfer to a healthy bank. Deposit insurance has virtually eliminated bank runs in the US since the 1930s.

```
DEPOSIT INSURANCE COVERAGE (US FDIC)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Ownership Category              │ Coverage Limit                         │
    │   ─────────────────────────────────│────────────────────────────────────────│
    │   Single accounts (individual)    │ $250,000                               │
    │   ─────────────────────────────────│────────────────────────────────────────│
    │   Joint accounts                  │ $250,000 per co-owner                 │
    │   ─────────────────────────────────│────────────────────────────────────────│
    │   Revocable trust accounts        │ $250,000 per beneficiary              │
    │   ─────────────────────────────────│────────────────────────────────────────│
    │   IRA and other retirement        │ $250,000                               │
    │   ─────────────────────────────────│────────────────────────────────────────│
    │   Corporation, partnership,       │ $250,000                               │
    │   unincorporated association      │                                        │
    │   ─────────────────────────────────│────────────────────────────────────────│
    │   Government accounts             │ $250,000                               │
    │                                                                             │
    │   Example: Individual with $250k in checking and $250k in savings         │
    │   at same bank in same ownership category: Only $250k insured.            │
    │   To get full coverage, spread across banks or ownership categories.      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
COMMERCIAL BANK FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Accounting Equation: Assets = Liabilities + Equity                       │
    │                                                                             │
    │   Net Interest Income = Interest Income - Interest Expense                 │
    │                                                                             │
    │   Net Interest Margin = NII / Average Earning Assets                       │
    │                                                                             │
    │   Return on Assets (ROA) = Net Income / Average Total Assets               │
    │                                                                             │
    │   Return on Equity (ROE) = Net Income / Average Equity                     │
    │                                                                             │
    │   Efficiency Ratio = Non-Interest Expense / Revenue                        │
    │                                                                             │
    │   Loan Loss Provision = Change in Allowance + Net Charge-Offs              │
    │                                                                             │
    │   Net Charge-Off Rate = (Gross Charge-Offs - Recoveries) / Average Loans   │
    │                                                                             │
    │   Capital Ratio (CET1) = CET1 Capital / Risk-Weighted Assets               │
    │                                                                             │
    │   Risk-Weighted Assets = Σ (Asset Value × Risk Weight)                     │
    │                                                                             │
    │   Liquidity Coverage Ratio = HQLA / Net Cash Outflows (30 days) ≥ 100%     │
    │                                                                             │
    │   Net Stable Funding Ratio = ASF / RSF ≥ 100%                              │
    │                                                                             │
    │   Tier 1 Leverage Ratio = Tier 1 Capital / Average Total Assets ≥ 4%       │
    │                                                                             │
    │   Gap (Rate Sensitivity) = RSA - RSL                                       │
    │                                                                             │
    │   Change in NII = Gap × ΔInterest Rate                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Commercial banks accept deposits, make loans, and process payments. They are financial intermediaries.

2. Core functions: deposit taking, lending, payment processing, maturity transformation, risk transformation, liquidity transformation.

3. Balance sheet: assets = liabilities + equity. Assets include loans, securities, reserves. Liabilities include deposits, borrowings.

4. Deposits are bank liabilities. Customers lend money to the bank when they deposit.

5. Loan loss reserve (allowance) is a contra-asset for expected future loan losses.

6. Equity (capital) is the loss-absorbing buffer. Protects depositors.

7. Money creation: banks create new deposits when making loans. No existing deposit is used.

8. Loan underwriting: Five C's (Character, Capacity, Capital, Collateral, Conditions).

9. Payment processing: banks debit payor accounts, credit payee accounts. Interbank settlement through central bank reserves.

10. Net interest income = interest earned minus interest paid. Primary revenue source (60-70%).

11. Non-interest income: fees from deposits, credit cards, mortgages, wealth management.

12. Credit risk: borrower defaults. Mitigated by underwriting, collateral, diversification, reserves, capital.

13. Liquidity risk: unable to meet withdrawal demands. Mitigated by liquid assets, LCR, NSFR, contingency plans.

14. Market risk: losses from interest rates, exchange rates, asset prices. Mitigated by hedging, limits.

15. Operational risk: internal failures, fraud, systems, external events. Mitigated by controls, insurance.

16. Basel III capital requirements: CET1 4.5% of RWA, Tier 1 6%, Total 8% plus buffers.

17. Risk-weighted assets: 0% for government bonds, 100% for corporate loans, higher for riskier assets.

18. Deposit insurance (FDIC) insures up to $250,000 per depositor, preventing runs.

19. Bank regulation: multiple agencies (Fed, OCC, FDIC, CFPB, state) oversee safety, soundness, consumer protection.

20. Key metrics: NIM, ROA, ROE, efficiency ratio, capital ratios, LCR, NSFR.

*This documentation belongs to https://github.com/InterCentury*
```