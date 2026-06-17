# Double-Entry Accounting

## Documentation Overview

Double-entry accounting is the foundational system of recording financial transactions in which every transaction affects at least two accounts, with equal debits and credits. This system ensures the accounting equation (Assets = Liabilities + Equity) always remains balanced. This document covers the principles, mechanics, accounts, rules, and applications of double-entry accounting in banking and finance.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the fundamental accounting equation                            │
    │   Learn the rules of debit and credit for each account type                 │
    │   Study the chart of accounts and account classification                    │
    │   Analyze the journal entry process and posting to ledgers                  │
    │   Examine the trial balance and financial statement preparation             │
    │   Understand the accounting cycle                                           │
    │   Learn banking-specific accounting applications                            │
    │   Study accrual accounting vs cash accounting                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## The Fundamental Accounting Equation

### The Core Identity

The accounting equation is the foundation of double-entry accounting. It must always balance.

```
THE ACCOUNTING EQUATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                    ASSETS = LIABILITIES + EQUITY                            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ASSETS                                                            │   │
    │   │   (What the entity owns)                                            │   │
    │   │                                                                     │   │
    │   │   ┌─────────────────────────────────────────────────────────────┐   │   │
    │   │   │ Cash, Accounts Receivable, Inventory, Equipment, Real       │   │   │
    │   │   │ Estate, Investments, Loans Receivable, Goodwill             │   │   │
    │   │   └─────────────────────────────────────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                    │                                        │
    │                                    │ =                                      │
    │                                    ▼                                        │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   LIABILITIES                    +    EQUITY                        │   │
    │   │   (What the entity owes)         (Owner's claim)                    │   │
    │   │                                                                     │   │
    │   │   ┌──────────────────────────┐   ┌──────────────────────────────┐   │   │
    │   │   │ Accounts Payable         │   │ Share Capital                │   │   │
    │   │   │ Loans Payable            │   │ Retained Earnings            │   │   │
    │   │   │ Deposits (for banks)     │   │ Dividends/Withdrawals        │   │   │
    │   │   │ Accrued Expenses         │   │ Net Income/Loss              │   │   │
    │   │   └──────────────────────────┘   └──────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Expanded Accounting Equation

The accounting equation can be expanded to show the relationship between revenue, expenses, and equity.

```
EXPANDED ACCOUNTING EQUATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ASSETS = LIABILITIES + OWNER'S EQUITY + (REVENUES - EXPENSES)             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │   
    │   │                                                                     │   │
    │   │   NET INCOME = REVENUES - EXPENSES                                  │   │
    │   │                                                                     │   │
    │   │   If Revenues > Expenses → Net Income → Increases Equity            │   │
    │   │   If Revenues < Expenses → Net Loss → Decreases Equity              │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   COMPLETE EQUATION:                                                        │
    │                                                                             │
    │   ASSETS = LIABILITIES + EQUITY + REVENUES - EXPENSES                       │
    │                                                                             │
    │   Or rearranged:                                                            │
    │                                                                             │
    │   ASSETS + EXPENSES = LIABILITIES + EQUITY + REVENUES                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Why Double-Entry Works

The system works because every transaction has two effects. Resources must always come from somewhere and go somewhere.

```
RESOURCE FLOW PRINCIPLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   EVERY TRANSACTION HAS:                                                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   SOURCE (Where resources come from)                                │   │
    │   │   │                                                                 │   │
    │   │   │   ┌─────────────────────────────────────────────────────────┐   │   │
    │   │   │   │ Liability increases (borrowed)                          │   │   │
    │   │   │   │ Liability decreases (repaid)                            │   │   │
    │   │   │   │ Equity increases (owner investment)                     │   │   │
    │   │   │   │ Equity decreases (withdrawal)                           │   │   │
    │   │   │   │ Revenue increases (income earned)                       │   │   │
    │   │   │   │ Expense decreases (cost reduction)                      │   │   │
    │   │   │   └─────────────────────────────────────────────────────────┘   │   │
    │   │   │                                                                 │   │
    │   │   │   VS.                                                           │   │
    │   │   │                                                                 │   │
    │   │   │   DESTINATION (Where resources go)                              │   │
    │   │   │                                                                 │   │
    │   │   │   ┌─────────────────────────────────────────────────────────┐   │   │
    │   │   │   │ Asset increases (acquired)                              │   │   │
    │   │   │   │ Asset decreases (sold/used)                             │   │   │
    │   │   │   │ Expense increases (cost incurred)                       │   │   │
    │   │   │   │ Revenue decreases (refunds/returns)                     │   │   │
    │   │   │   └─────────────────────────────────────────────────────────┘   │   │
    │   │   │                                                                 │   │
    │   │   └─────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   The total value of all sources must equal the total value of all          │
    │   destinations.                                                             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## The Rules of Debit and Credit

### Debit and Credit Effects by Account Type

Each account type has specific rules for increases and decreases.

```
DEBIT AND CREDIT RULES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ACCOUNT TYPE        │ DEBIT (dr)         │ CREDIT (cr)        │ NORMAL    │
    │                       │                    │                    │ BALANCE   │
    │   ────────────────────│────────────────────│────────────────────│────────── │
    │   Assets              │ Increase (+)       │ Decrease (-)       │ Debit     │
    │   ────────────────────│────────────────────│────────────────────│────────── │
    │   Liabilities         │ Decrease (-)       │ Increase (+)       │ Credit    │
    │   ────────────────────│────────────────────│────────────────────│────────── │
    │   Equity (Capital)    │ Decrease (-)       │ Increase (+)       │ Credit    │
    │   ────────────────────│────────────────────│────────────────────│────────── │
    │   Revenue (Income)    │ Decrease (-)       │ Increase (+)       │ Credit    │
    │   ────────────────────│────────────────────│────────────────────│────────── │
    │   Expenses (Costs)    │ Increase (+)       │ Decrease (-)       │ Debit     │
    │   ────────────────────│────────────────────│────────────────────│────────── │
    │   Dividends /         │ Increase (+)       │ Decrease (-)       │ Debit     │
    │   Withdrawals         │                    │                    │           │
    │                                                                             │
    │                                                                             │
    │   MNEMONIC: DEAD CLIC                                                       │
    │                                                                             │
    │   DEBITS INCREASE:  Expense, Asset, Dividend/Withdrawal                     │
    │   CREDITS INCREASE:  Liability, Capital/Equity, Income/Revenue              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### T-Account Visualization

T-accounts visually represent how debits and credits affect each account.

```
T-ACCOUNT STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                      ┌─────────────────────────┐                            │
    │                      │     ACCOUNT NAME        │                            │
    │                      ├──────────────┬──────────┤                            │
    │                      │   DEBIT      │  CREDIT  │                            │
    │                      │   (Left)     │  (Right) │                            │
    │                      ├──────────────┼──────────┤                            │
    │                      │              │          │                            │
    │                      │    Increases │ Decreases│  (Asset / Expense)         │
    │                      │              │          │                            │
    │                      │    Decreases │ Increases│  (Liability / Equity /     │
    │                      │              │          │   Revenue)                 │
    │                      │              │          │                            │
    │                      ├──────────────┼──────────┤                            │
    │                      │    Total     │ Total    │                            │
    │                      │    Debits    │ Credits  │                            │
    │                      └──────────────┴──────────┘                            │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE: CASH (Asset) T-Account                                           │
    │                                                                             │
    │                      ┌─────────────────────────┐                            │
    │                      │         CASH            │                            │
    │                      ├──────────────┬──────────┤                            │
    │                      │   DEBIT      │  CREDIT  │                            │
    │                      ├──────────────┼──────────┤                            │
    │                      │   $1,000     │   $200   │                            │
    │                      │   $500       │   $300   │                            │
    │                      │   $250       │   $100   │                            │
    │                      │              │          │                            │
    │                      │   $1,750     │   $600   │                            │
    │                      ├──────────────┼──────────┤                            │
    │                      │   Balance    │          │                            │
    │                      │   $1,150     │          │                            │
    │                      │   (Debit)    │          │                            │
    │                      └──────────────┴──────────┘                            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### The Golden Rule of Double-Entry

Every transaction must have equal total debits and total credits.

```
GOLDEN RULE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TOTAL DEBITS = TOTAL CREDITS                                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   TRANSACTION: Depositing $1000 cash into the bank                  │   │
    │   │                                                                     │   │
    │   │   ┌─────────────────────────────────────────────────────────────┐   │   │
    │   │   │  Account                     │ Debit ($)  │ Credit ($)      │   │   │
    │   │   │  ────────────────────────────│────────────│─────────────────│   │   │
    │   │   │  Cash (Asset)                │ 1,000      │                 │   │   │
    │   │   │  Bank Deposit (Asset)        │            │ 1,000           │   │   │
    │   │   │  ────────────────────────────│────────────│─────────────────│   │   │
    │   │   │  TOTAL                       │ 1,000      │ 1,000           │   │   │
    │   │   └─────────────────────────────────────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   TRANSACTION: Borrowing $5000 from the bank                        │   │
    │   │                                                                     │   │
    │   │   ┌─────────────────────────────────────────────────────────────┐   │   │
    │   │   │  Account                     │ Debit ($)  │ Credit ($)      │   │   │
    │   │   │  ────────────────────────────│────────────│─────────────────│   │   │
    │   │   │  Cash (Asset)                │ 5,000      │                 │   │   │
    │   │   │  Bank Loan (Liability)       │            │ 5,000           │   │   │
    │   │   │  ────────────────────────────│────────────│─────────────────│   │   │
    │   │   │  TOTAL                       │ 5,000      │ 5,000           │   │   │
    │   │   └─────────────────────────────────────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Chart of Accounts

### Account Classification Structure

The chart of accounts is a complete listing of all accounts used by an entity, organized by category.

```
CHART OF ACCOUNTS STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ACCOUNT NUMBER RANGE           │ ACCOUNT TYPE                             │
    │   ───────────────────────────────│───────────────────────────────────────── │
    │   1000 - 1999                    │ ASSETS                                   │
    │                                  │                                          │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  1100 Cash in Vault                                                 │   │
    │   │  1110 Reserves at Central Bank                                      │   │
    │   │  1120 Cash in ATM                                                   │   │
    │   │  1200 Loans Receivable                                              │   │
    │   │  1210 Commercial Loans                                              │   │
    │   │  1220 Real Estate Loans                                             │   │
    │   │  1230 Consumer Loans                                                │   │
    │   │  1240 Loan Loss Reserve (Contra-Asset)                              │   │
    │   │  1300 Securities                                                    │   │
    │   │  1310 Treasury Securities                                           │   │
    │   │  1320 Municipal Securities                                          │   │
    │   │  1400 Fixed Assets                                                  │   │
    │   │  1410 Bank Premises                                                 │   │
    │   │  1420 Equipment                                                     │   │
    │   │  1430 Accumulated Depreciation (Contra-Asset)                       │   │
    │   │  1500 Other Assets                                                  │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   2000 - 2999                    LIABILITIES                                │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  2100 Deposits                                                      │   │
    │   │  2110 Demand Deposits (Checking)                                    │   │
    │   │  2120 Savings Deposits                                              │   │
    │   │  2130 Time Deposits (CDs)                                           │   │
    │   │  2140 NOW Accounts                                                  │   │
    │   │  2200 Borrowings                                                    │   │
    │   │  2210 Federal Funds Purchased                                       │   │
    │   │  2220 Discount Window Loans                                         │   │
    │   │  2300 Accrued Expenses                                              │   │
    │   │  2400 Other Liabilities                                             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   3000 - 3999                    EQUITY                                     │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  3100 Share Capital                                                 │   │
    │   │  3200 Retained Earnings                                             │   │
    │   │  3300 Dividends Declared                                            │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   4000 - 4999                    REVENUE                                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  4100 Interest Income                                               │   │
    │   │  4110 Loan Interest                                                 │   │
    │   │  4120 Securities Interest                                           │   │
    │   │  4200 Fee Income                                                    │   │
    │   │  4210 Account Maintenance Fees                                      │   │
    │   │  4220 ATM Fees                                                      │   │
    │   │  4230 Overdraft Fees                                                │   │
    │   │  4300 Trading Income                                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   5000 - 5999                    EXPENSES                                   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  5100 Interest Expense                                              │   │
    │   │  5110 Deposit Interest                                              │   │
    │   │  5120 Borrowing Interest                                            │   │
    │   │  5200 Personnel Expenses                                            │   │
    │   │  5210 Salaries and Wages                                            │   │
    │   │  5220 Benefits                                                      │   │
    │   │  5300 Operating Expenses                                            │   │
    │   │  5310 Rent                                                          │   │
    │   │  5320 Utilities                                                     │   │
    │   │  5330 Insurance                                                     │   │
    │   │  5400 Loan Loss Provision                                           │   │
    │   │  5500 Depreciation                                                  │   │
    │   │  5600 Other Expenses                                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Bank-Specific Accounts

Banks have unique accounts not found in non-financial businesses.

```
BANK-SPECIFIC ACCOUNT TYPES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ACCOUNT                   │ TYPE          │ DESCRIPTION                   │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Reserves at Central Bank  │ Asset         │ Digital account at central    │
    │                             │               │ bank for settlement           │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Loans Receivable          │ Asset         │ Amounts owed by borrowers     │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Loan Loss Reserve         │ Contra-Asset  │ Estimated losses on loans     │
    │   (Allowance)               │               │                               │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Deposits                  │ Liability     │ Amounts owed to depositors    │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Interest Accrued          │ Asset         │ Interest earned but not       │
    │   Receivable                │               │ yet received                  │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Interest Accrued Payable  │ Liability     │ Interest owed but not yet     │
    │                             │               │ paid                          │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Fed Funds Purchased       │ Liability     │ Overnight borrowings from     │
    │                             │               │ other banks                   │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Fed Funds Sold            │ Asset         │ Overnight loans to other      │
    │                             │               │ banks                         │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Trading Securities        │ Asset         │ Securities held for short-    │
    │                             │               │ term trading                  │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Available-for-Sale        │ Asset         │ Securities held for           │
    │   Securities                │               │ liquidity/investment          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Journal Entries

### The Journal Entry Format

Journal entries are recorded in a standardized format showing date, accounts, debits, credits, and description.

```
JOURNAL ENTRY FORMAT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Date: 2024-06-15                                                          │
    │   Description: Customer deposit of $1000 cash into checking account         │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash in Vault (Asset)       │ 1,000      │                         │   │
    │   │  Demand Deposits (Liability) │            │ 1,000                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Reference: JE-2024-0615-001                                               │
    │   Posted By: TELLER_JSMITH                                                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Common Banking Transactions

```
COMMON BANKING JOURNAL ENTRIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TRANSACTION 1: Customer deposits $1000 cash into checking                 │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash in Vault (Asset)       │ 1,000      │                         │   │
    │   │  Demand Deposits (Liability) │            │ 1,000                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Effect: Assets increase, Liabilities increase                             │
    │                                                                             │
    │                                                                             │
    │   TRANSACTION 2: Bank makes $5000 loan to customer                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Loans Receivable (Asset)    │ 5,000      │                         │   │
    │   │  Demand Deposits (Liability) │            │ 5,000                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Effect: Assets increase, Liabilities increase (new money creation)        │
    │                                                                             │
    │                                                                             │
    │   TRANSACTION 3: Customer transfers $200 from checking to savings           │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Demand Deposits (Liability) │ 200        │                         │   │
    │   │  Savings Deposits (Liability)│            │ 200                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Effect: One liability decreases, another liability increases            │
    │   Total liabilities unchanged                                              │
    │                                                                             │
    │                                                                             │
    │   TRANSACTION 4: Customer withdraws $200 cash from ATM                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Demand Deposits (Liability) │ 200        │                         │   │
    │   │  Cash in Vault (Asset)       │            │ 200                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Effect: Assets decrease, Liabilities decrease                           │
    │                                                                             │
    │                                                                             │
    │   TRANSACTION 5: Bank pays $100 interest on deposit                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Interest Expense (Expense)  │ 100        │                         │   │
    │   │  Demand Deposits (Liability) │            │ 100                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Effect: Expenses increase (reduces equity), Liabilities increase         │
    │                                                                             │
    │                                                                             │
    │   TRANSACTION 6: Bank collects $300 interest on a loan                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash (Asset)                │ 300        │                         │   │
    │   │  Interest Income (Revenue)   │            │ 300                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Effect: Assets increase, Revenue increases (increases equity)           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Compound Journal Entries

Some transactions involve more than two accounts.

```
COMPOUND JOURNAL ENTRIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TRANSACTION: Customer deposits $1000 cash and $300 check                 │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash in Vault (Asset)       │ 1,000      │                         │   │
    │   │  Checks in Collection        │ 300        │                         │   │
    │   │  (Asset)                     │            │                         │   │
    │   │  Demand Deposits (Liability) │            │ 1,300                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Total Debits = $1,300, Total Credits = $1,300                           │
    │                                                                             │
    │                                                                             │
    │   TRANSACTION: Bank makes $10,000 loan with $100 origination fee          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Loans Receivable (Asset)    │ 10,000     │                         │   │
    │   │  Cash (Asset)                │            │ 10,000                  │   │
    │   │  Cash (Asset)                │ 100        │                         │   │
    │   │  Fee Income (Revenue)        │            │ 100                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Total Debits = $10,100, Total Credits = $10,100                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Posting to the Ledger

### The Posting Process

After journal entries are recorded, they are posted to individual accounts in the general ledger.

```
POSTING PROCESS FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   JOURNAL ENTRY                                                            │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash (Asset)                │ 1,000      │                         │   │
    │   │  Deposits (Liability)        │            │ 1,000                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ├──────────────────────────────────────────────────────────────────┐ │
    │        │                                                                  │ │
    │        ▼                                                                  ▼ │
    │   ┌─────────────────────┐          ┌─────────────────────────────────────┐ │
    │   │   CASH LEDGER       │          │   DEPOSITS LEDGER                   │ │
    │   ├──────────────┬──────┤          ├──────────────┬──────────────────────┤ │
    │   │   DEBIT      │CREDIT│          │   DEBIT      │ CREDIT               │ │
    │   ├──────────────┼──────┤          ├──────────────┼──────────────────────┤ │
    │   │   $1,000     │      │          │              │ $1,000               │ │
    │   ├──────────────┼──────┤          ├──────────────┼──────────────────────┤ │
    │   │   Bal: $1,000│      │          │              │ Bal: $1,000          │ │
    │   └──────────────┴──────┘          └──────────────┴──────────────────────┘ │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Ledger Account Format

```
LEDGER ACCOUNT FORMAT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Account Name: Cash in Vault                                              │
    │   Account Number: 1100                                                     │
    │   Account Type: Asset                                                      │
    │                                                                             │
    │   ┌───────┬──────────────┬────────────┬──────────┬────────────┬───────────┐│
    │   │ Date  │ Description  │ Reference  │ Debit    │ Credit     │ Balance   ││
    │   ├───────┼──────────────┼────────────┼──────────┼────────────┼───────────┤│
    │   │ 6/1   │ Opening      │            │          │            │ 10,000    ││
    │   │ 6/3   │ Deposit      │ JE-001     │ 1,000    │            │ 11,000    ││
    │   │ 6/5   │ ATM Withdraw │ JE-004     │          │ 200        │ 10,800    ││
    │   │ 6/7   │ Deposit      │ JE-006     │ 500      │            │ 11,300    ││
    │   │ 6/9   │ Wire Out     │ JE-008     │          │ 300        │ 11,000    ││
    │   │ 6/12  │ Deposit      │ JE-010     │ 2,000    │            │ 13,000    ││
    │   │ 6/15  │ ATM Withdraw │ JE-012     │          │ 150        │ 12,850    ││
    │   ├───────┼──────────────┼────────────┼──────────┼────────────┼───────────┤│
    │   │       │ Total        │            │ 3,500    │ 650        │ 12,850    ││
    │   └───────┴──────────────┴────────────┴──────────┴────────────┴───────────┘│
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Trial Balance

### Purpose of Trial Balance

The trial balance lists all accounts and their balances to verify that total debits equal total credits.

```
TRIAL BALANCE FORMAT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ABC BANK                                                                 │
    │   Trial Balance                                                             │
    │   As of June 30, 2024                                                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account #   │ Account Name               │ Debit ($)  │ Credit ($) │   │
    │   │  ────────────│────────────────────────────│────────────│────────────│   │
    │   │  1100        │ Cash in Vault              │ 12,850     │            │   │
    │   │  1110        │ Reserves at Central Bank   │ 25,000     │            │   │
    │   │  1200        │ Loans Receivable           │ 150,000    │            │   │
    │   │  1240        │ Loan Loss Reserve          │            │ 1,500      │   │
    │   │  1300        │ Securities                 │ 75,000     │            │   │
    │   │  1400        │ Bank Premises              │ 50,000     │            │   │
    │   │  1430        │ Acc. Depreciation          │            │ 10,000     │   │
    │   │  2100        │ Deposits                   │            │ 200,000    │   │
    │   │  2200        │ Borrowings                 │            │ 50,000     │   │
    │   │  3100        │ Share Capital              │            │ 40,000     │   │
    │   │  3200        │ Retained Earnings          │            │ 15,000     │   │
    │   │  4100        │ Interest Income            │            │ 8,500      │   │
    │   │  4200        │ Fee Income                 │            │ 2,500      │   │
    │   │  5100        │ Interest Expense           │ 2,000      │            │   │
    │   │  5200        │ Personnel Expenses         │ 8,000      │            │   │
    │   │  5300        │ Operating Expenses         │ 4,650      │            │   │
    │   │  5400        │ Loan Loss Provision        │ 1,000      │            │   │
    │   ├──────────────┼────────────────────────────┼────────────┼────────────┤   │
    │   │              │ TOTAL                      │ 328,500    │ 328,500    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Total Debits = Total Credits = $328,500                                  │
    │   ✓ Trial balance is in balance                                             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Adjusting Entries

Adjusting entries are made at period end to record accruals, deferrals, and estimates.

```
ADJUSTING ENTRIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ACCRUAL ENTRY: Interest earned but not received                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Interest Accrued Receivable │ 500        │                         │   │
    │   │  (Asset)                     │            │                         │   │
    │   │  Interest Income (Revenue)   │            │ 500                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   ACCRUAL ENTRY: Interest owed but not paid                               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Interest Expense (Expense)  │ 300        │                         │   │
    │   │  Interest Accrued Payable    │            │ 300                     │   │
    │   │  (Liability)                 │            │                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   DEFERRAL ENTRY: Prepaid insurance used during period                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Insurance Expense (Expense) │ 200        │                         │   │
    │   │  Prepaid Insurance (Asset)   │            │ 200                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   ESTIMATE ENTRY: Loan loss provision                                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Loan Loss Provision         │ 1,000      │                         │   │
    │   │  (Expense)                   │            │                         │   │
    │   │  Loan Loss Reserve (Contra-  │            │ 1,000                   │   │
    │   │  Asset)                      │            │                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Financial Statement Preparation

### Income Statement

The income statement shows revenues, expenses, and net income over a period.

```
INCOME STATEMENT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ABC BANK                                                                 │
    │   Income Statement                                                          │
    │   For the Month Ended June 30, 2024                                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │  REVENUES                                                           │   │
    │   │  ├── Interest Income                         $8,500                │   │
    │   │  ├── Fee Income                              $2,500                │   │
    │   │  ├── Trading Income                          $1,000                │   │
    │   │  ├── Other Income                            $500                  │   │
    │   │  │                                                                 │   │
    │   │  │  Total Revenues                           $12,500              │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  EXPENSES                                                           │   │
    │   │  ├── Interest Expense                         $2,000                │   │
    │   │  ├── Personnel Expenses                       $8,000                │   │
    │   │  ├── Operating Expenses                       $4,650                │   │
    │   │  ├── Loan Loss Provision                      $1,000                │   │
    │   │  ├── Depreciation                             $500                  │   │
    │   │  ├── Other Expenses                           $350                  │   │
    │   │  │                                                                 │   │
    │   │  │  Total Expenses                            $16,500              │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  NET INCOME (LOSS)                            ($4,000)             │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Balance Sheet

The balance sheet shows assets, liabilities, and equity at a point in time.

```
BALANCE SHEET

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ABC BANK                                                                 │
    │   Balance Sheet                                                             │
    │   As of June 30, 2024                                                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ASSETS                                                             │   │
    │   │  ├── Cash and Cash Equivalents                                      │   │
    │   │  │   ├── Cash in Vault                       $12,850                │   │
    │   │  │   └── Reserves at Central Bank            $25,000                │   │
    │   │  │                                           $37,850                │   │
    │   │  ├── Loans (Net of LLR)                      $148,500               │   │
    │   │  │   ├── Gross Loans                         $150,000               │   │
    │   │  │   └── Less: Loan Loss Reserve             ($1,500)               │   │
    │   │  ├── Securities                               $75,000               │   │
    │   │  ├── Fixed Assets (Net of Depreciation)       $40,000               │   │
    │   │  │   ├── Bank Premises                        $50,000               │   │
    │   │  │   └── Less: Acc. Depreciation             ($10,000)              │   │
    │   │  ├── Other Assets                             $5,000                │   │
    │   │  │                                                                 │   │
    │   │  │  TOTAL ASSETS                              $306,350              │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  LIABILITIES                                                         │   │
    │   │  ├── Deposits                                 $200,000              │   │
    │   │  ├── Borrowings                                $50,000              │   │
    │   │  ├── Accrued Expenses                          $2,000               │   │
    │   │  ├── Other Liabilities                         $1,350               │   │
    │   │  │                                                                 │   │
    │   │  │  TOTAL LIABILITIES                          $253,350             │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  EQUITY                                                              │   │
    │   │  ├── Share Capital                             $40,000              │   │
    │   │  ├── Retained Earnings (Beginning)             $15,000              │   │
    │   │  └── Net Loss (Current Period)                 ($4,000)             │   │
    │   │  │                                                                 │   │
    │   │  │  TOTAL EQUITY                               $51,000              │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  TOTAL LIABILITIES AND EQUITY                  $304,350              │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Statement of Cash Flows

The statement of cash flows shows cash inflows and outflows by activity.

```
STATEMENT OF CASH FLOWS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ABC BANK                                                                 │
    │   Statement of Cash Flows                                                   │
    │   For the Month Ended June 30, 2024                                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │  OPERATING ACTIVITIES                                               │   │
    │   │  ├── Net Income (Loss)                         ($4,000)             │   │
    │   │  ├── Adjustments for non-cash items:                                │   │
    │   │  │   ├── Loan Loss Provision                   $1,000               │   │
    │   │  │   ├── Depreciation                         $500                 │   │
    │   │  ├── Changes in operating assets/liabilities:                       │   │
    │   │  │   ├── Increase in Loans                     ($10,000)            │   │
    │   │  │   ├── Increase in Deposits                  $15,000              │   │
    │   │  │   ├── Increase in Accrued Expenses          $500                 │   │
    │   │  │                                                                 │   │
    │   │  │  Net Cash from Operating Activities         $3,000               │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  INVESTING ACTIVITIES                                               │   │
    │   │  ├── Purchase of Securities                    ($5,000)             │   │
    │   │  ├── Purchase of Premises                      ($2,000)             │   │
    │   │  │                                                                 │   │
    │   │  │  Net Cash from Investing Activities         ($7,000)             │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  FINANCING ACTIVITIES                                               │   │
    │   │  ├── Proceeds from Borrowings                  $5,000               │   │
    │   │  ├── Dividends Paid                            ($500)               │   │
    │   │  │                                                                 │   │
    │   │  │  Net Cash from Financing Activities         $4,500               │   │
    │   │  ────────────────────────────────────────────────────────────────── │   │
    │   │                                                                     │   │
    │   │  NET INCREASE IN CASH                            $500               │   │
    │   │  ├── Beginning Cash Balance                     $37,350              │   │
    │   │  ├── Ending Cash Balance                        $37,850              │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Accrual vs Cash Accounting

### Comparison of Methods

```
ACCRUAL VS CASH ACCOUNTING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FEATURE              │ ACCRUAL ACCOUNTING    │ CASH ACCOUNTING           │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Revenue Recognition  │ When earned           │ When cash received        │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Expense Recognition  │ When incurred         │ When cash paid            │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Matching Principle   │ Matches revenues to   │ No matching required      │
    │                        │ expenses in same      │                           │
    │                        │ period                │                           │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Timing Differences   │ Accruals and          │ No accruals               │
    │                        │ deferrals             │                           │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Complexity           │ Complex               │ Simple                    │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Required by GAAP     │ Yes (for large       │ No (only small entities)   │
    │                        │ entities)            │                           │
    │   ─────────────────────│───────────────────────│───────────────────────────│
    │   Used by Banks        │ Yes                   │ No                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Example Comparison

```
ACCRUAL VS CASH EXAMPLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TRANSACTION: Bank earns $1000 interest on loan in December,              │
    │   customer pays in January                                                 │
    │                                                                             │
    │                                                                             │
    │   ACCRUAL ACCOUNTING (December):                                           │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Interest Accrued Receivable │ 1,000      │                         │   │
    │   │  (Asset)                     │            │                         │   │
    │   │  Interest Income (Revenue)   │            │ 1,000                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Result: Revenue recognized in December (when earned)                    │
    │   Asset recorded for amount due                                             │
    │                                                                             │
    │                                                                             │
    │   ACCRUAL ACCOUNTING (January - when cash received):                       │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash (Asset)                │ 1,000      │                         │   │
    │   │  Interest Accrued Receivable │            │ 1,000                   │   │
    │   │  (Asset)                     │            │                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Result: Cash increases, asset decreases. No revenue recorded.            │
    │                                                                             │
    │                                                                             │
    │   CASH ACCOUNTING:                                                         │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Cash (Asset)                │ 1,000      │                         │   │
    │   │  Interest Income (Revenue)   │            │ 1,000                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Result: Revenue recognized in January (when cash received)              │
    │   No asset for unpaid amounts recorded                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## The Accounting Cycle

### Complete Cycle Flow

The accounting cycle is the complete process of recording and reporting financial information.

```
ACCOUNTING CYCLE FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   START: Transactions Occur                                                 │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 1: Analyze Transactions                                             │
    │   ├── Identify affected accounts                                           │
    │   ├── Determine debit and credit effects                                   │
    │   └── Verify accounting equation remains balanced                         │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 2: Record Journal Entries (Journalizing)                           │
    │   ├── Chronological record of transactions                                │
    │   ├── Date, accounts, amounts, description                                 │
    │   └── Documented with supporting evidence                                 │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 3: Post to General Ledger (Posting)                                │
    │   ├── Transfer journal entries to ledger accounts                         │
    │   ├── Update account balances                                              │
    │   └── Creates T-accounts for each account                                 │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 4: Prepare Unadjusted Trial Balance                                │
    │   ├── List all accounts with balances                                     │
    │   ├── Verify total debits = total credits                                 │
    │   └── Identify any errors                                                  │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 5: Record Adjusting Entries                                        │
    │   ├── Accruals (revenue/expense not yet recorded)                         │
    │   ├── Deferrals (prepaid/uneared items)                                   │
    │   ├── Estimates (depreciation, loan losses)                               │
    │   └── Required for accrual accounting                                     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 6: Prepare Adjusted Trial Balance                                  │
    │   ├── After adjusting entries                                              │
    │   ├── Verify debits = credits                                              │
    │   └── Used to prepare financial statements                                │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 7: Prepare Financial Statements                                    │
    │   ├── Income Statement (Revenue - Expenses = Net Income)                 │
    │   ├── Statement of Retained Earnings                                      │
    │   ├── Balance Sheet (Assets = Liabilities + Equity)                      │
    │   └── Statement of Cash Flows                                             │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 8: Record Closing Entries                                          │
    │   ├── Close revenue accounts to Income Summary                            │
    │   ├── Close expense accounts to Income Summary                           │
    │   ├── Close Income Summary to Retained Earnings                          │
    │   └── Close Dividends to Retained Earnings                                │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 9: Prepare Post-Closing Trial Balance                             │
    │   ├── Only permanent accounts (assets, liabilities, equity)              │
    │   ├── Temporary accounts (revenue, expense, dividends) zeroed out       │
    │   └── Verify debits = credits                                             │
    │        │                                                                   │
    │        ▼                                                                   │
    │   NEXT PERIOD: Repeat Cycle                                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Closing Entries

Closing entries reset temporary accounts to zero for the next accounting period.

```
CLOSING ENTRIES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STEP 1: Close Revenue accounts to Income Summary                         │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Interest Income (Revenue)   │ 8,500      │                         │   │
    │   │  Fee Income (Revenue)        │ 2,500      │                         │   │
    │   │  Trading Income (Revenue)    │ 1,000      │                         │   │
    │   │  Other Income (Revenue)      │ 500        │                         │   │
    │   │  Income Summary              │            │ 12,500                  │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   STEP 2: Close Expense accounts to Income Summary                         │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Income Summary              │ 16,500     │                         │   │
    │   │  Interest Expense            │            │ 2,000                   │   │
    │   │  Personnel Expenses          │            │ 8,000                   │   │
    │   │  Operating Expenses          │            │ 4,650                   │   │
    │   │  Loan Loss Provision         │            │ 1,000                   │   │
    │   │  Depreciation                │            │ 500                     │   │
    │   │  Other Expenses              │            │ 350                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   STEP 3: Close Income Summary to Retained Earnings                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Income Summary              │            │ 4,000                   │   │
    │   │  (Net Loss - see below)      │            │                         │   │
    │   │  Retained Earnings           │ 4,000      │                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Note: Since Net Loss = $4,000, Retained Earnings is debited.            │
    │   If Net Income, Retained Earnings would be credited.                     │
    │                                                                             │
    │                                                                             │
    │   STEP 4: Close Dividends to Retained Earnings                            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account                     │ Debit ($)  │ Credit ($)              │   │
    │   │  ────────────────────────────│────────────│─────────────────────────│   │
    │   │  Retained Earnings           │ 500        │                         │   │
    │   │  Dividends Declared          │            │ 500                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
DOUBLE-ENTRY ACCOUNTING FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Basic Equation: Assets = Liabilities + Equity                            │
    │                                                                             │
    │   Expanded Equation: Assets = Liabilities + Equity + Revenues - Expenses   │
    │                                                                             │
    │   Net Income = Revenues - Expenses                                         │
    │                                                                             │
    │   Equity, Ending = Equity, Beginning + Net Income - Dividends              │
    │                                                                             │
    │   Total Debits = Total Credits (Every transaction)                         │
    │                                                                             │
    │   Trial Balance: Σ(Debits) = Σ(Credits)                                    │
    │                                                                             │
    │   Loan Net Value = Gross Loans - Loan Loss Reserve                         │
    │                                                                             │
    │   Book Value = Asset Cost - Accumulated Depreciation                       │
    │                                                                             │
    │   Working Capital = Current Assets - Current Liabilities                   │
    │                                                                             │
    │   Retained Earnings, Ending = Retained Earnings, Beginning +               │
    │   Net Income - Dividends                                                   │
    │                                                                             │
    │   Return on Equity (ROE) = Net Income / Average Equity                     │
    │                                                                             │
    │   Return on Assets (ROA) = Net Income / Average Assets                     │
    │                                                                             │
    │   Debt-to-Equity Ratio = Total Liabilities / Total Equity                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Double-entry accounting: every transaction affects at least two accounts with equal debits and credits.

2. Accounting equation: Assets = Liabilities + Equity. Must always balance.

3. Expanded equation: Assets + Expenses = Liabilities + Equity + Revenues.

4. Debits increase: Assets, Expenses, Dividends (DEAD). Credits increase: Liabilities, Equity, Revenue (CLIC).

5. T-accounts visually show debits (left) and credits (right) for each account.

6. Normal balances: Assets/Expenses/Dividends = Debit; Liabilities/Equity/Revenue = Credit.

7. Chart of accounts organizes accounts by type: Assets (1000s), Liabilities (2000s), Equity (3000s), Revenue (4000s), Expenses (5000s).

8. Bank-specific accounts: Reserves at central bank, loans receivable, loan loss reserve, deposits, fed funds.

9. Journal entries record transactions chronologically with date, accounts, debits, credits, description.

10. Compound entries involve more than two accounts. Total debits still equal total credits.

11. Posting transfers journal entries to ledger accounts.

12. Trial balance verifies total debits = total credits. Detects errors.

13. Adjusting entries: accruals, deferrals, estimates (depreciation, loan loss).

14. Financial statements: Income Statement, Balance Sheet, Statement of Cash Flows.

15. Accrual accounting: revenue when earned, expenses when incurred (GAAP required).

16. Cash accounting: revenue when received, expenses when paid (simple, not GAAP).

17. Accounting cycle: analyze → journalize → post → trial balance → adjust → adjusted trial balance → statements → close → post-closing trial balance.

18. Closing entries: close revenue and expenses to income summary, close income summary to retained earnings.

19. Temporary accounts (revenue, expense, dividends) reset to zero each period.

20. Permanent accounts (assets, liabilities, equity) carry balances forward.

*This documentation belongs to https://github.com/InterCentury*
```