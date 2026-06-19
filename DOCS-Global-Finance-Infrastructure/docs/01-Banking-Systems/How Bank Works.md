# How Banks Work

## Documentation Overview

A bank is a financial institution that accepts deposits from the public, creates credit, and facilitates the flow of money through the economy. Banks are the primary engines of money creation, payment processing, and financial intermediation. This document explains the complete operation of a bank: how it takes deposits, makes loans, creates money, processes payments, communicates with other banks, manages risks, and earns profits—all within the regulatory framework.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the complete banking business model                           │
    │   Learn how banks accept deposits and make loans                           │
    │   Study the money creation mechanism                                       │
    │   Analyze interbank communication and settlement                           │
    │   Examine payment processing and clearing systems                          │
    │   Understand bank profitability and revenue sources                        │
    │   Study bank risk management                                               │
    │   Learn the role of central banks in banking                               │
    │   Understand bank regulation and supervision                               │
    │   Examine the future of banking                                            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## The Banking Business Model

### Core Business: Financial Intermediation

Banks are financial intermediaries that bridge the gap between savers (depositors) and borrowers. This is the fundamental business model.

How it works: Savers deposit money into banks seeking safety and modest returns. Borrowers seek funds for consumption or investment. The bank collects deposits from many savers, pools them, and lends to borrowers. The bank earns profit from the spread between what it pays on deposits and what it charges on loans.

```
BANK AS FINANCIAL INTERMEDIARY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                    ┌─────────────────────────────────────┐                  │
    │                    │                                     │                  │
    │   ┌─────────────┐  │   ┌─────────────────────────────┐  │  ┌─────────────┐  │
    │   │   SAVERS    │  │   │           BANK              │  │  │  BORROWERS  │  │
    │   │(Depositors) │  │   │                             │  │  │             │  │
    │   │             │──┼──►│  Deposits (Liabilities)     │──┼──►│ Loans       │  │
    │   │  Households │  │   │  Loans (Assets)             │  │  │ (Principal  │  │
    │   │  Businesses │  │   │  Net Interest Margin        │  │  │ + Interest) │  │
    │   │  Government │  │   │  Fees and Services          │  │  │  Households │  │
    │   └─────────────┘  │   └─────────────────────────────┘  │  │  Businesses │  │
    │                    │                                     │  │  Government │  │
    │                    └─────────────────────────────────────┘  └─────────────┘  │
    │                                                                             │
    │                                                                             │
    │   KEY FLOWS:                                                               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Savers → Bank: Deposits (money flows in)                           │   │
    │   │  Bank → Savers: Interest payments (money flows out)                  │   │
    │   │  Bank → Borrowers: Loans (money flows out)                           │   │
    │   │  Borrowers → Bank: Loan repayments (money flows in)                  │   │
    │   │  Bank → Bank: Profit from interest spread                            │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Transformation Services

Banks perform three critical transformations that make the financial system work.

```
THREE TRANSFORMATIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TRANSFORMATION 1: MATURITY TRANSFORMATION                               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Depositors want short-term access:                                 │   │
    │   │   ├── Checking accounts (immediate withdrawal)                      │   │
    │   │   ├── Savings accounts (instant access)                             │   │
    │   │   └── Short-term CDs (days to months)                              │   │
    │   │                                                                     │   │
    │   │   Borrowers want long-term funds:                                   │   │
    │   │   ├── Mortgages (15-30 years)                                       │   │
    │   │   ├── Business loans (5-10 years)                                   │   │
    │   │   └── Equipment financing (3-7 years)                              │   │
    │   │                                                                     │   │
    │   │   Bank transforms short-term deposits into long-term loans.         │   │
    │   │   This is the core function of banking.                             │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   TRANSFORMATION 2: LIQUIDITY TRANSFORMATION                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Loans are illiquid: Cannot be easily sold for cash               │   │
    │   │   Deposits are liquid: Can be withdrawn on demand                   │   │
    │   │                                                                     │   │
    │   │   Bank transforms illiquid loans into liquid deposits.              │   │
    │   │   Depositors get liquidity. Borrowers get long-term funds.         │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   TRANSFORMATION 3: RISK TRANSFORMATION                                   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Borrowers have credit risk: They might default                   │   │
    │   │   Depositors want safety: They want guaranteed returns              │   │
    │   │                                                                     │   │
    │   │   Bank transforms risky loans into safe deposits.                   │   │
    │   │   Bank absorbs credit risk through:                                 │   │
    │   │   ├── Diversification (many borrowers)                              │   │
    │   │   ├── Underwriting (credit analysis)                                │   │
    │   │   ├── Collateral (security)                                         │   │
    │   │   ├── Loan loss reserves (provisions)                               │   │
    │   │   └── Capital (equity buffer)                                       │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Simple Balance Sheet Model

At its simplest, a bank's balance sheet is:

```
SIMPLE BANK BALANCE SHEET

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ABC BANK                                                                 │
    │   Balance Sheet                                                             │
    │                                                                             │
    │   ┌─────────────────────────────┐   ┌─────────────────────────────┐        │
    │   │          ASSETS             │   │        LIABILITIES           │        │
    │   │                             │   │                             │        │
    │   │  ┌───────────────────────┐  │   │  ┌───────────────────────┐  │        │
    │   │  │ Reserves (10%)        │  │   │  │ Deposits (100%)       │  │        │
    │   │  │ $10 million           │  │   │  │ $100 million          │  │        │
    │   │  └───────────────────────┘  │   │  └───────────────────────┘  │        │
    │   │                             │   │                             │        │
    │   │  ┌───────────────────────┐  │   │  ┌───────────────────────┐  │        │
    │   │  │ Loans (90%)           │  │   │  │ Equity (Capital)      │  │        │
    │   │  │ $90 million           │  │   │  │ $10 million           │  │        │
    │   │  └───────────────────────┘  │   │  └───────────────────────┘  │        │
    │   │                             │   │                             │        │
    │   │  ┌───────────────────────┐  │   │                             │        │
    │   │  │ TOTAL ASSETS          │  │   │  ┌───────────────────────┐  │        │
    │   │  │ $100 million          │  │   │  │ TOTAL LIABILITIES +   │  │        │
    │   │  └───────────────────────┘  │   │  │ EQUITY                │  │        │
    │   │                             │   │  │ $100 million          │  │        │
    │   │                             │   │  └───────────────────────┘  │        │
    │   └─────────────────────────────┘   └─────────────────────────────┘        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Deposit Taking

### How Deposits Work

When a customer deposits money, the bank creates a liability (it owes the customer) and gains an asset (cash or reserves).

How it works: Customer brings $1000 cash. Bank adds $1000 to vault cash (asset) and credits customer's deposit account (liability). The bank now owes the customer $1000. This is the foundation of banking—accepting deposits creates the raw material for lending.

```
DEPOSIT PROCESS FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER DEPOSITS $1000 CASH                                             │
    │                                                                             │
    │   STEP 1: Customer brings cash to bank                                     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 2: Teller counts and verifies cash                                  │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 3: Bank credits customer's account                                  │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Customer Account Ledger                                             │   │
    │   │  ├── Customer: John Smith                                           │   │
    │   │  ├── Account #: 12345678                                            │   │
    │   │  ├── Transaction: Deposit                                           │   │
    │   │  ├── Amount: +$1,000                                                │   │
    │   │  └── New Balance: $5,234.67                                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 4: Bank updates balance sheet                                      │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Ledger                                                         │   │
    │   │  ├── Vault Cash (Asset): +$1,000                                    │   │
    │   │  └── Customer Deposits (Liability): +$1,000                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 5: Customer receives receipt and sees updated balance              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Types of Deposits

```
DEPOSIT TYPES AND CHARACTERISTICS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DEPOSIT TYPE       │ INTEREST   │ LIQUIDITY    │ COST TO BANK            │
    │   ───────────────────│────────────│──────────────│─────────────────────────│
    │   Checking (Demand)  │ 0-0.1%     │ Immediate    │ Lowest cost             │
    │   (Non-interest)     │            │              │ (check processing fees) │
    │   ───────────────────│────────────│──────────────│─────────────────────────│
    │   Interest Checking  │ 0.1-0.5%   │ Immediate    │ Low cost                │
    │   (NOW Accounts)     │            │              │                         │
    │   ───────────────────│────────────│──────────────│─────────────────────────│
    │   Savings Accounts   │ 0.5-2%     │ Immediate    │ Moderate cost           │
    │   ───────────────────│────────────│──────────────│─────────────────────────│
    │   Money Market       │ 1-3%       │ Limited      │ Moderate cost           │
    │   Deposit Accounts   │            │ checks       │                         │
    │   ───────────────────│────────────│──────────────│─────────────────────────│
    │   Certificates of    │ 2-5%       │ Penalty for  │ Higher cost             │
    │   Deposit (CDs)      │            │ early        │                         │
    │                      │            │ withdrawal   │                         │
    │   ───────────────────│────────────│──────────────│─────────────────────────│
    │   Jumbo CDs (>$100k) │ 3-6%       │ Penalty for  │ Highest cost            │
    │                      │            │ early        │                         │
    │                      │            │ withdrawal   │                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Lending and Money Creation

### How Lending Works

When a bank makes a loan, it does not lend out existing deposits. It creates a new deposit in the borrower's account. This is the money creation mechanism.

How it works: Bank approves a $10,000 loan. The bank adds $10,000 to loans receivable (asset) and credits the borrower's deposit account (liability). No existing deposit is used. New money is created. The bank has created money from nothing (except the borrower's promise to repay).

```
MONEY CREATION THROUGH LENDING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BEFORE LOAN:                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                   │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Deposits: $100,000          │   │   │
    │   │  │ Loans: $0                   ││ │ Equity: $10,000             │   │   │
    │   │  └─────────────────────────────┘│ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply (deposits) = $100,000                                       │
    │                                                                             │
    │                                                                             │
    │   BANK APPROVES $20,000 LOAN:                                              │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank Assets                    │ Bank Liabilities                   │   │
    │   │  ┌─────────────────────────────┐│ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $10,000           ││ │ Deposits: $120,000          │   │   │
    │   │  │ Loans: $20,000 (new)        ││ │   (+$20,000 created)        │   │   │
    │   │  └─────────────────────────────┘│ │ Equity: $10,000             │   │   │
    │   │                                │ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Money supply (deposits) = $120,000 (+$20,000 new money)                  │
    │                                                                             │
    │   KEY INSIGHT: Banks create money through lending. No deposit             │
    │   is used. The loan creates a new deposit.                                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Loan Approval Process

```
LOAN APPROVAL PROCESS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STEP 1: Application                                                      │
    │   ├── Customer completes loan application                                 │
    │   ├── Provides financial information                                      │
    │   └── Specifies loan purpose                                               │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 2: Credit Check                                                     │
    │   ├── Pull credit report (FICO, VantageScore)                             │
    │   ├── Check bankruptcy history                                             │
    │   ├── Verify employment and income                                         │
    │   └── Calculate debt-to-income ratio                                       │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 3: Underwriting (Five C's)                                          │
    │   ├── Character: Credit history                                            │
    │   ├── Capacity: Ability to repay                                           │
    │   ├── Capital: Down payment/equity                                         │
    │   ├── Collateral: Security for loan                                        │
    │   └── Conditions: Purpose, economic environment                            │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 4: Decision                                                         │
    │   ├── Approve (with conditions)                                            │
    │   ├── Counter-offer (different terms)                                      │
    │   └── Decline                                                              │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 5: Closing                                                          │
    │   ├── Sign loan documents                                                 │
    │   ├── Funds disbursed to borrower's account                                │
    │   └── New money created                                                    │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## How Banks Communicate with Each Other

### Interbank Communication Systems

Banks communicate using secure, standardized messaging systems to transfer funds, settle obligations, and share information.

```
INTERBANK COMMUNICATION CHANNELS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CHANNEL 1: SWIFT (Society for Worldwide Interbank Financial              │
    │   Telecommunication)                                                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ┌─────────────┐     ┌─────────────────┐     ┌─────────────┐      │   │
    │   │   │   Bank A    │────►│  SWIFT Network  │────►│   Bank B    │      │   │
    │   │   │   (Sender)  │     │   (Secure      │     │ (Receiver)  │      │   │
    │   │   │             │◄────│    Messaging)   │◄────│             │      │   │
    │   │   └─────────────┘     └─────────────────┘     └─────────────┘      │   │
    │   │                                                                     │   │
    │   │   Uses: Payment instructions, trade confirmations, messages        │   │
    │   │   Format: ISO 20022 (modern), MT messages (legacy)                  │   │
    │   │   Security: PKI encryption, authentication                          │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   CHANNEL 2: RTGS (Real-Time Gross Settlement)                             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ┌─────────────┐     ┌─────────────────┐     ┌─────────────┐      │   │
    │   │   │   Bank A    │────►│  Central Bank   │────►│   Bank B    │      │   │
    │   │   │   (Payer)   │     │  RTGS System    │     │ (Payee)     │      │   │
    │   │   │             │◄────│   (Fedwire,     │◄────│             │      │   │
    │   │   │             │     │    TARGET2)     │     │             │      │   │
    │   │   └─────────────┘     └─────────────────┘     └─────────────┘      │   │
    │   │                                                                     │   │
    │   │   Settlement is final and irrevocable                                │   │
    │   │   Uses central bank reserves                                         │   │
    │   │   Real-time settlement                                                │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   CHANNEL 3: ACH (Automated Clearing House)                                │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ┌─────────────┐     ┌─────────────────┐     ┌─────────────┐      │   │
    │   │   │   Bank A    │────►│  Clearing       │────►│   Bank B    │      │   │
    │   │   │ (Originating│     │  House (NACHA)  │     │ (Receiving) │      │   │
    │   │   │  Bank)      │◄────│                 │◄────│             │      │   │
    │   │   └─────────────┘     └─────────────────┘     └─────────────┘      │   │
    │   │                                                                     │   │
    │   │   Batch processing (end of day settlement)                          │   │
    │   │   Used for direct deposits, bill payments, payroll                  │   │
    │   │   Lower cost, slower than RTGS                                       │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   CHANNEL 4: Fedwire / CHAPS / TARGET2 (RTGS Systems)                     │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ┌─────────────────────────────────────────────────────────────┐   │   │
    │   │   │   Country        │ System Name    │ Operator                 │   │   │
    │   │   │   ──────────────│────────────────│──────────────────────────│   │   │
    │   │   │   United States │ Fedwire        │ Federal Reserve           │   │   │
    │   │   │   Eurozone      │ TARGET2        │ Eurosystem                │   │   │
    │   │   │   United Kingdom│ CHAPS          │ Bank of England           │   │   │
    │   │   │   Japan         │ BOJ-NET        │ Bank of Japan             │   │   │
    │   │   │   China         │ CNAPS          │ People's Bank of China    │   │   │
    │   │   └─────────────────────────────────────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Complete Cross-Border Payment Flow

```
CROSS-BORDER PAYMENT PROCESS (USD Transfer)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER IN UK SENDS $10,000 TO CUSTOMER IN US                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   STEP 1: UK Customer initiates transfer at UK Bank                │   │
    │   │   ├── Provides US bank details (ABA routing #, account #)          │   │
    │   │   ├── Approves $10,000 + $50 fee                                    │   │
    │   │   └── UK Bank debits customer account                               │   │
    │   │                                                                     │   │
    │   │   STEP 2: UK Bank sends SWIFT MT103 message                         │   │
    │   │   ├── To: US Correspondent Bank (or direct to US Bank)             │   │
    │   │   ├── Via: SWIFT network                                            │   │
    │   │   └── Contains: Amount, Beneficiary, Originator                     │   │
    │   │                                                                     │   │
    │   │   STEP 3: Correspondent Banking                                     │   │
    │   │   ├── UK Bank debits its nostro account at US Correspondent        │   │
    │   │   ├── US Correspondent credits US Bank's account                   │   │
    │   │   └── US Correspondent sends MT103 to US Bank                      │   │
    │   │                                                                     │   │
    │   │   STEP 4: US Bank processes incoming payment                        │   │
    │   │   ├── Verify MT103 message                                           │   │
    │   │   ├── Credit customer's account                                     │   │
    │   │   └── Send confirmation                                             │   │
    │   │                                                                     │   │
    │   │   STEP 5: Settlement                                                │   │
    │   │   ├── Via Fedwire: UK Bank's correspondent sends USD               │   │
    │   │   │   to US Bank's correspondent                                    │   │
    │   │   └── Final settlement in central bank reserves                     │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   DIAGRAM:                                                                 │
    │                                                                             │
    │   ┌─────────────┐  SWIFT     ┌─────────────────┐  Fedwire   ┌─────────────┐│
    │   │  UK Bank    │───────────►│ US Correspondent │───────────►│   US Bank   ││
    │   │             │  MT103     │      Bank        │  Reserve   │             ││
    │   │  (Sender)   │◄───────────│                  │◄───────────│  (Receiver) ││
    │   └─────────────┘            └─────────────────┘            └─────────────┘│
    │        │                           │                           │           │
    │        │ Debit                     │ Nostro/Vostro             │ Credit    │
    │        ▼                           ▼                           ▼           │
    │   Customer A                                                  Customer B   │
    │   (Payer)                                                    (Payee)      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Correspondent Banking

Smaller banks cannot directly access foreign payment systems. They use larger correspondent banks.

```
CORRESPONDENT BANKING RELATIONSHIP

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Community Bank (Small)                                            │   │
    │   │   ├── No direct access to SWIFT                                    │   │
    │   │   ├── No foreign currency accounts                                 │   │
    │   │   └── No direct access to foreign payment systems                  │   │
    │   │                                                                     │   │
    │   │                    │                                               │   │
    │   │                    │ Correspondent relationship                    │   │
    │   │                    │ (Nostro account)                              │   │
    │   │                    ▼                                               │   │
    │   │   ┌─────────────────────────────────────────────────────────────┐   │   │
    │   │   │                                                              │   │   │
    │   │   │   Correspondent Bank (Large)                                 │   │   │
    │   │   │   ├── SWIFT member                                           │   │   │
    │   │   │   ├── Holds USD, EUR, GBP accounts                           │   │   │
    │   │   │   ├── Direct access to Fedwire, TARGET2, CHAPS              │   │   │
    │   │   │   └── Serves 1,000+ community banks                          │   │   │
    │   │   │                                                              │   │   │
    │   │   └─────────────────────────────────────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   NOSTRO ACCOUNT: Account held by local bank at correspondent bank        │
    │   VOSTRO ACCOUNT: Account held by correspondent bank at local bank        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Payment Processing

### Complete Payment Flow

Every payment follows a similar path through the banking system.

```
PAYMENT PROCESSING: DEBIT CARD TRANSACTION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CUSTOMER BUYS $100 OF GROCERIES WITH DEBIT CARD                         │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   STEP 1: Authorization                                            │   │
    │   │   ├── Customer swipes card at POS                                  │   │
    │   │   ├── Merchant terminal sends to acquirer                          │   │
    │   │   ├── Acquirer sends to card network (Visa/Mastercard)              │   │
    │   │   ├── Card network sends to issuing bank                           │   │
    │   │   ├── Issuing bank verifies funds and sends approval               │   │
    │   │   └── Authorization flows back to terminal                         │   │
    │   │                                                                     │   │
    │   │   STEP 2: Clearing                                                  │   │
    │   │   ├── Merchant submits batch of transactions                        │   │
    │   │   ├── Acquirer sends clearing file to card network                 │   │
    │   │   ├── Card network distributes to issuing banks                    │   │
    │   │   └── Issuing banks verify and accept                               │   │
    │   │                                                                     │   │
    │   │   STEP 3: Settlement                                                │   │
    │   │   ├── Card network calculates net positions                        │   │
    │   │   ├── Issues settlement instructions to banks                      │   │
    │   │   ├── Issuing banks transfer funds to acquirers                   │   │
    │   │   └── Acquirers credit merchant accounts                            │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   FLOW DIAGRAM:                                                            │
    │                                                                             │
    │   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐                   │
    │   │  Customer   │───►│  Merchant   │───►│  Acquirer   │                   │
    │   │  (Cardholder)│    │  (Store)    │    │  (Bank)     │                   │
    │   └─────────────┘    └─────────────┘    └──────┬──────┘                   │
    │         ▲                           ▲          │                           │
    │         │                           │          │                           │
    │         │                           │          ▼                           │
    │   ┌─────────────┐              ┌─────────────┐                           │
    │   │  Issuing    │◄─────────────│   Card      │                           │
    │   │   Bank      │              │   Network   │                           │
    │   │             │─────────────►│  (Visa/MC)  │                           │
    │   └─────────────┘              └─────────────┘                           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Settlement Finality

Settlement finality means that once a payment is settled, it is irreversible. This is crucial for banking operations.

```
SETTLEMENT FINALITY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   SETTLEMENT FINALITY: The point at which a payment becomes               │
    │   irrevocable and cannot be reversed.                                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   RTGS Settlement (Fedwire, TARGET2)                                │   │
    │   │   ├── Finality: Immediate                                           │   │
    │   │   ├── Risk: None (central bank reserves)                            │   │
    │   │   └── Legal: Irrevocable upon settlement                           │   │
    │   │                                                                     │   │
    │   │   ACH Settlement (Batch)                                            │   │
    │   │   ├── Finality: End of day                                          │   │
    │   │   ├── Risk: Intraday credit exposure                                │   │
    │   │   └── Legal: Reversible until settlement                            │   │
    │   │                                                                     │   │
    │   │   Card Settlement (Visa/Mastercard)                                 │   │
    │   │   ├── Finality: 1-3 days                                            │   │
    │   │   ├── Risk: Chargebacks possible                                    │   │
    │   │   └── Legal: Reversible for 60-120 days                            │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Bank Profitability

### Revenue Sources

Banks earn money through two primary channels: net interest income and non-interest income.

```
BANK REVENUE SOURCES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   REVENUE SOURCE 1: NET INTEREST INCOME (60-70% of revenue)               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Interest Earned (on assets)                                       │   │
    │   │   ├── Loan interest: 6-12% depending on loan type                  │   │
    │   │   ├── Securities interest: 3-5%                                    │   │
    │   │   ├── Fed funds sold: 5-6%                                         │   │
    │   │   └── Other earning assets: 4-8%                                   │   │
    │   │                                                                     │   │
    │   │   Interest Paid (on liabilities)                                    │   │
    │   │   ├── Deposit interest: 0-5% depending on product                  │   │
    │   │   ├── Borrowing interest: 5-6%                                     │   │
    │   │   └── Other interest: 4-8%                                         │   │
    │   │                                                                     │   │
    │   │   Net Interest Income = Interest Earned - Interest Paid            │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   REVENUE SOURCE 2: NON-INTEREST INCOME (30-40% of revenue)               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Deposit Fees                                                      │   │
    │   │   ├── Monthly maintenance fees                                      │   │
    │   │   ├── Overdraft fees                                                │   │
    │   │   ├── ATM fees                                                      │   │
    │   │   └── NSF fees                                                      │   │
    │   │                                                                     │   │
    │   │   Lending Fees                                                      │   │
    │   │   ├── Origination fees                                              │   │
    │   │   ├── Late payment fees                                             │   │
    │   │   └── Prepayment penalties                                          │   │
    │   │                                                                     │   │
    │   │   Card Fees                                                         │   │
    │   │   ├── Interchange fees (merchant processing)                        │   │
    │   │   ├── Annual credit card fees                                       │   │
    │   │   └── Foreign transaction fees                                      │   │
    │   │                                                                     │   │
    │   │   Wealth Management Fees                                            │   │
    │   │   ├── Investment advisory fees                                      │   │
    │   │   ├── Asset management fees                                         │   │
    │   │   └── Brokerage commissions                                         │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Net Interest Margin

Net Interest Margin (NIM) is the difference between interest earned and interest paid, as a percentage of earning assets.

```
NET INTEREST MARGIN CALCULATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FORMULA: NIM = (Interest Income - Interest Expense) / Earning Assets     │
    │                                                                             │
    │   EXAMPLE BANK:                                                            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Assets (Earning)                         Amount   Yield            │   │
    │   │  ────────────────────────────────────────│─────────│────────────────│   │
    │   │  Loans                                     $500M    7.0%            │   │
    │   │  Securities                                 $200M    4.0%            │   │
    │   │  Other earning assets                       $100M    5.0%            │   │
    │   │  Total Earning Assets                      $800M                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Interest Income = ($500M × 7%) + ($200M × 4%) + ($100M × 5%) = $48M      │
    │   Yield on Earning Assets = $48M / $800M = 6.0%                            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Liabilities (Interest-bearing)          Amount   Rate              │   │
    │   │  ────────────────────────────────────────│─────────│────────────────│   │
    │   │  Deposits                                  $600M    2.0%            │   │
    │   │  Borrowings                                 $100M    5.0%            │   │
    │   │  Total Interest-Bearing Liabilities        $700M                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Interest Expense = ($600M × 2%) + ($100M × 5%) = $17M                    │
    │   Cost of Funds = $17M / $700M = 2.43%                                     │
    │                                                                             │
    │   Net Interest Income = $48M - $17M = $31M                                 │
    │   Net Interest Margin = $31M / $800M = 3.88%                               │
    │                                                                             │
    │   Industry average NIM: 3.0-4.5% (varies by bank size, business model)    │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

### Efficiency Ratio

The efficiency ratio measures how much it costs to generate revenue.

```
EFFICIENCY RATIO

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FORMULA: Efficiency Ratio = Non-Interest Expense / Revenue               │
    │                                                                             │
    │   Non-Interest Expense includes:                                           │
    │   ├── Personnel costs (salaries, benefits, bonuses)                        │
    │   ├── Occupancy costs (rent, utilities, maintenance)                       │
    │   ├── Technology costs (hardware, software, IT staff)                      │
    │   ├── Marketing and advertising                                            │
    │   ├── Legal and compliance                                                 │
    │   └── Other operating expenses                                             │
    │                                                                             │
    │   EXAMPLE:                                                                 │
    │                                                                             │
    │   Non-Interest Expense = $20 million                                       │
    │   Revenue (Net Interest Income + Non-Interest Income) = $40 million        │
    │   Efficiency Ratio = $20M / $40M = 50%                                    │
    │                                                                             │
    │   Lower is better:                                                         │
    │   ├── 50-60%: Good, well-managed bank                                     │
    │   ├── 60-70%: Average                                                     │
    │   └── >70%: Inefficient, cost pressures                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

## Risk Management

### Types of Bank Risks

Banks face multiple types of risks that must be managed.

```
BANK RISK TYPES AND MITIGATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   RISK 1: CREDIT RISK (Risk of borrower default)                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Mitigation:                                                         │   │
    │   │  ├── Rigorous underwriting (Five C's)                               │   │
    │   │  ├── Diversification (many borrowers, industries)                    │   │
    │   │  ├── Collateral requirements                                         │   │
    │   │  ├── Credit scoring and monitoring                                   │   │
    │   │  ├── Loan loss reserves (provisions)                                 │   │
    │   │  └── Capital buffer (equity)                                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RISK 2: LIQUIDITY RISK (Cannot meet withdrawal demands)                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Mitigation:                                                         │   │
    │   │  ├── Liquid asset buffer (cash, Treasuries)                         │   │
    │   │  ├── Liquidity Coverage Ratio (LCR ≥ 100%)                          │   │
    │   │  ├── Net Stable Funding Ratio (NSFR ≥ 100%)                         │   │
    │   │  ├── Contingency funding plan                                        │   │
    │   │  ├── Access to central bank discount window                         │   │
    │   │  └── Federal funds market access                                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RISK 3: MARKET RISK (Changes in interest rates, FX, asset prices)       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Mitigation:                                                         │   │
    │   │  ├── Interest rate hedging (swaps, futures)                          │   │
    │   │  ├── Asset-liability management (ALM)                                │   │
    │   │  ├── Gap analysis (rate-sensitive assets vs liabilities)             │   │
    │   │  ├── Duration matching                                               │   │
    │   │  ├── Value at Risk (VaR) limits                                     │   │
    │   │  └── Stress testing                                                  │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RISK 4: OPERATIONAL RISK (Internal failures, fraud, systems)            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Mitigation:                                                         │   │
    │   │  ├── Internal controls and segregation of duties                    │   │
    │   │  ├── Cybersecurity measures                                         │   │
    │   │  ├── Business continuity planning                                    │   │
    │   │  ├── Employee training                                              │   │
    │   │  ├── Insurance coverage                                              │   │
    │   │  └── Regular audits                                                  │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

### Capital Requirements

Banks must maintain minimum capital to absorb unexpected losses.

```
CAPITAL REQUIREMENTS (Basel III)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CAPITAL TIERS:                                                           │
    │                                                                             │
    │   Common Equity Tier 1 (CET1)                                              │
    │   ├── Highest quality capital                                               │
    │   ├── Common shares + retained earnings                                    │
    │   └── Minimum: 4.5% of Risk-Weighted Assets (RWA)                         │
    │                                                                             │
    │   Additional Tier 1 (AT1)                                                  │
    │   ├── Preferred stock, contingent convertible bonds (CoCos)               │
    │   └── Minimum: 1.5% of RWA                                                 │
    │                                                                             │
    │   Tier 2 Capital                                                           │
    │   ├── Subordinated debt, loan loss reserves (limited)                      │
    │   └── Minimum: 2.0% of RWA                                                 │
    │                                                                             │
    │   Total Capital Requirement = 8.0% of RWA (minimum)                       │
    │   Plus buffers: Capital Conservation (2.5%), Countercyclical (0-2.5%)      │
    │                                                                             │
    │   Typical Total Capital for well-capitalized bank: 10-15% of RWA          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

## Role of Central Banks

### Central Bank Functions

Central banks are the ultimate backstop and regulator of the banking system.

```
CENTRAL BANK FUNCTIONS IN BANKING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FUNCTION 1: MONETARY POLICY                                              │
    │   ├── Set policy rate (interest on reserves)                              │
    │   ├── Control money supply through open market operations                 │
    │   ├── Influence lending rates throughout economy                          │
    │   └── Target inflation (usually 2%)                                       │
    │                                                                             │
    │   FUNCTION 2: BANKER TO BANKS                                              │
    │   ├── Maintain reserve accounts for commercial banks                      │
    │   ├── Provide settlement services (RTGS)                                   │
    │   ├── Clear interbank payments                                             │
    │   └── Hold bank reserves (vault cash + central bank deposits)             │
    │                                                                             │
    │   FUNCTION 3: LENDER OF LAST RESORT                                        │
    │   ├── Provide emergency liquidity (discount window)                       │
    │   ├── Prevent bank runs                                                    │
    │   ├── Maintain financial stability                                         │
    │   └── Bagehot's principle: lend freely at penalty rate                    │
    │                                                                             │
    │   FUNCTION 4: REGULATION AND SUPERVISION                                   │
    │   ├── Examine banks for safety and soundness                              │
    │   ├── Enforce capital requirements (Basel III)                            │
    │   ├── Conduct stress tests                                                │
    │   └── Close insolvent banks                                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

### Bank-Central Bank Relationship

```
BANK-CENTRAL BANK INTERACTION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                     COMMERCIAL BANK                                  │   │
    │   │                                                                     │   │
    │   │   Holds reserves at central bank                                   │   │
    │   │   Borrows from central bank (discount window)                       │   │
    │   │   Sends payments through central bank RTGS                         │   │
    │   │   Complies with central bank regulations                            │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                     │                                      │
    │                                     │ Interaction                           │
    │                                     ▼                                      │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                     CENTRAL BANK                                     │   │
    │   │                                                                     │   │
    │   │   Sets policy rate                                                  │   │
    │   │   Holds bank reserves                                               │   │
    │   │   Provides settlement                                               │   │
    │   │   Lender of last resort                                             │   │
    │   │   Regulator and supervisor                                          │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   INTERACTION TYPES:                                                       │
    │                                                                             │
    │   Daily: Bank settles payments through central bank RTGS                  │
    │   Weekly: Bank monitors reserve balances against requirements             │
    │   Monthly: Bank reports to central bank (balance sheet, loans, deposits)  │
    │   Quarterly: Bank submits regulatory filings                              │
    │   Annually: Bank undergoes examination by central bank                    │
    │   Crisis: Bank borrows from central bank discount window                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

## Regulation and Supervision

### Regulatory Framework

Banks are heavily regulated to ensure safety, soundness, and consumer protection.

```
BANK REGULATORY BODIES (US Example)

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

### Bank Examination

Regulators conduct regular examinations to assess bank safety and soundness.

```
CAMELS RATING SYSTEM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CAMELS COMPONENT               │ WHAT IS EVALUATED                       │
    │   ───────────────────────────────│─────────────────────────────────────────│
    │   C: Capital Adequacy            │ Capital levels, capital ratios,         │
    │                                  │ ability to absorb losses                │
    │   ───────────────────────────────│─────────────────────────────────────────│
    │   A: Asset Quality               │ Loan quality, non-performing loans,    │
    │                                  │ loan loss reserves                      │
    │   ───────────────────────────────│─────────────────────────────────────────│
    │   M: Management                  │ Management quality, risk culture,       │
    │                                  │ governance, strategic planning          │
    │   ───────────────────────────────│─────────────────────────────────────────│
    │   E: Earnings                    │ Profitability, net interest margin,    │
    │                                  │ earnings trends                         │
    │   ───────────────────────────────│─────────────────────────────────────────│
    │   L: Liquidity                   │ Liquid assets, LCR, funding sources,   │
    │                                  │ access to markets                       │
    │   ───────────────────────────────│─────────────────────────────────────────│
    │   S: Sensitivity to Market Risk  │ Interest rate risk, FX risk,           │
    │                                  │ hedging practices                       │
    │                                                                             │
    │   Ratings: 1 (Strong) to 5 (Critically Deficient)                         │
    │   Rating 1-2: Sound banks                                                   │
    │   Rating 3: Weak, requires attention                                       │
    │   Rating 4-5: Serious problems, regulatory action                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

## Complete Bank Operations Summary

### How a Bank Works: The Complete Cycle

```
COMPLETE BANK OPERATIONS CYCLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   START: Depositors bring money to bank                            │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank accepts deposits (creates liabilities)                       │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank holds reserves (vault cash + central bank deposits)         │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank makes loans (creates new deposits, new money)               │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Borrowers spend money                                             │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Money circulates through economy                                 │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Payments processed through banking system                        │   │
    │   │   ├── Internal: Bank ledger updates                                │   │
    │   │   ├── Interbank: SWIFT, RTGS, ACH                                 │   │
    │   │   └── Central bank: Final settlement                               │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank earns revenue (interest + fees)                            │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank manages risks                                               │   │
    │   │   ├── Credit: Underwriting, monitoring, reserves                  │   │
    │   │   ├── Liquidity: Asset buffer, funding sources                    │   │
    │   │   ├── Market: Hedging, ALM                                        │   │
    │   │   └── Operational: Controls, cybersecurity                        │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank complies with regulation                                    │   │
    │   │   ├── Capital requirements (Basel III)                           │   │
    │   │   ├── Examinations (CAMELS)                                      │   │
    │   │   ├── Consumer protection (CFPB)                                 │   │
    │   │   └── Anti-money laundering (AML)                               │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank reports to stakeholders                                     │   │
    │   │   ├── Financial statements (GAAP)                                 │   │
    │   │   ├── Regulatory reports                                           │   │
    │   │   └── Shareholder reports                                          │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank distributes profits                                         │   │
    │   │   ├── Retained earnings (build capital)                           │   │
    │   │   └── Dividends (return to shareholders)                           │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Cycle continues                                                  │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

## Formulas Quick Reference

```
BANK OPERATIONS FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Net Interest Income = Interest Income - Interest Expense                 │
    │                                                                             │
    │   Net Interest Margin = NII / Average Earning Assets                       │
    │                                                                             │
    │   Efficiency Ratio = Non-Interest Expense / Revenue                        │
    │                                                                             │
    │   Return on Assets = Net Income / Average Total Assets                     │
    │                                                                             │
    │   Return on Equity = Net Income / Average Equity                           │
    │                                                                             │
    │   Loan Loss Reserve = Estimated Expected Losses on Loans                   │
    │                                                                             │
    │   Capital Ratio (CET1) = CET1 Capital / Risk-Weighted Assets               │
    │                                                                             │
    │   Liquidity Coverage Ratio = HQLA / Net Cash Outflows (30 days)            │
    │                                                                             │
    │   Net Stable Funding Ratio = Available Stable Funding / Required Stable    │
    │   Funding                                                                  │
    │                                                                             │
    │   Loan-to-Deposit Ratio = Total Loans / Total Deposits                     │
    │                                                                             │
    │   Tier 1 Leverage Ratio = Tier 1 Capital / Average Total Assets            │
    │                                                                             │
    │   Gap (Rate Sensitivity) = RSA - RSL                                       │
    │                                                                             │
    │   Change in NII = Gap × ΔInterest Rate                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
    ```

## Summary

1. Banks are financial intermediaries that transform deposits into loans, creating money in the process.

2. Three transformations: maturity (short deposits to long loans), liquidity (illiquid loans to liquid deposits), risk (risky loans to safe deposits).

3. Deposits are liabilities (bank owes customers), loans are assets (customers owe bank).

4. Money creation: banks create new deposits when making loans. No existing deposit is used.

5. Banks communicate via SWIFT (messaging), RTGS (settlement), ACH (batch), and correspondent banking.

6. Payments flow: authorization → clearing → settlement.

7. Revenue sources: Net Interest Income (60-70%) and Non-Interest Income (30-40%).

8. Net Interest Margin (NIM): 3.0-4.5% typical. Interest spread = core profitability.

9. Risk types: Credit, Liquidity, Market, Operational. Each requires specific mitigation.

10. Capital requirements: Basel III (CET1 4.5%, Tier 1 6%, Total 8% of RWA).

11. Central bank functions: monetary policy, banker to banks, lender of last resort, regulation.

12. Bank examination: CAMELS rating (Capital, Asset quality, Management, Earnings, Liquidity, Sensitivity).

13. Deposit insurance (FDIC): protects deposits up to $250,000, prevents runs.

14. Regulatory framework: multiple agencies (Fed, OCC, FDIC, CFPB, state).

15. Correspondent banking: smaller banks use larger banks for international access.

16. Nostro account: local bank's account at correspondent bank.

17. Settlement finality: RTGS immediate irrevocable. ACH end of day. Card reversible.

18. Efficiency ratio: lower is better (50-60% good, >70% inefficient).

19. Complete cycle: deposits → reserves → loans → spending → payments → revenue → risk management → regulation → distribution.

20. Banks are the engine of the modern economy. They create money, process payments, and allocate capital.

*This documentation belongs to https://github.com/InterCentury*
```