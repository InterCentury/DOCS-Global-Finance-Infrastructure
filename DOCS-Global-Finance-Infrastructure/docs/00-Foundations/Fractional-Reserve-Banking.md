# 05 - Fractional Reserve Banking

## Documentation Overview

Fractional reserve banking is a banking system in which banks hold only a fraction of their deposit liabilities as reserves, lending out the remainder to borrowers. This system allows banks to create money through the lending process, expanding the money supply beyond the base currency issued by the central bank. This document covers the mechanics, money creation process, reserve requirements, risks, and regulatory frameworks of fractional reserve banking.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand fractional reserve banking definition and mechanics          │
    │   Learn the distinction between reserves and deposits                      │
    │   Study the money creation process through lending                         │
    │   Analyze the money multiplier formula and its limitations                 │
    │   Examine reserve requirement ratios across jurisdictions                  │
    │   Understand bank runs and liquidity risk                                  │
    │   Learn deposit insurance and lender of last resort functions              │
    │   Study capital requirements and prudential regulation                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Core Concepts

### What is Fractional Reserve Banking

Fractional reserve banking is a system where banks are required to hold only a specified fraction of their deposit liabilities as reserves. The remaining deposits are available for lending to borrowers. This contrasts with full reserve banking, where banks would hold 100% of deposits as reserves and lend only from equity capital.

How it works: A customer deposits $1000 into a bank. The reserve requirement is 10%. The bank holds $100 as reserves and lends out $900 to a borrower. The $900 is deposited into another bank, which holds $90 as reserves and lends out $810. This process continues, multiplying the original deposit into a larger total money supply.

```
FULL RESERVE VS FRACTIONAL RESERVE COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FULL RESERVE BANKING (100% Reserve)                                      │
    │                                                                             │
    │   Depositor                                                               │
    │       │                                                                   │
    │       │ $1000 deposit                                                     │
    │       ▼                                                                   │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                              BANK                                    │   │
    │   │                                                                     │   │
    │   │   RESERVES: $1000          LOANS: $0                                │   │
    │   │   (100% of deposits)       (0% of deposits)                         │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Total Money Supply = $1000 (original deposit only)                      │
    │                                                                             │
    │                                                                             │
    │   FRACTIONAL RESERVE BANKING (10% Reserve)                                 │
    │                                                                             │
    │   Depositor                                                               │
    │       │                                                                   │
    │       │ $1000 deposit                                                     │
    │       ▼                                                                   │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                              BANK                                    │   │
    │   │                                                                     │   │
    │   │   RESERVES: $100            LOANS: $900                             │   │
    │   │   (10% of deposits)         (90% of deposits)                       │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │       │                                                                   │
    │       │ $900 loan                                                         │
    │       ▼                                                                   │
    │   Borrower spends $900 → Merchant deposits $900 → Bank B                 │
    │                                                                             │
    │   Total Money Supply = $1000 + $900 + $810 + ... = up to $10,000          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Reserves vs Deposits

Reserves: Funds that a bank holds either as physical cash in its vault or as deposits at the central bank. These are the most liquid assets and are used to meet depositor withdrawals and payment obligations.

Deposits: Liabilities of the bank to its depositors. When a customer deposits money, the bank records a liability equal to the deposit amount and acquires an asset (the reserves or loan).

How it works: A bank's balance sheet must always balance. When a bank receives a deposit, its liabilities (deposits) increase, and its assets (reserves) increase by the same amount. When the bank makes a loan, its assets (loans) increase, and it creates a new deposit (liability) for the borrower. This simultaneously increases both sides of the balance sheet, creating new money.

```
BANK BALANCE SHEET TRANSACTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   INITIAL DEPOSIT ($1000)                                                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ASSETS                          LIABILITIES                        │   │
    │   │  ┌─────────────────────────────┐ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: +$1000            │ │ Deposits: +$1000             │   │   │
    │   │  └─────────────────────────────┘ └─────────────────────────────┘   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   AFTER MEETING RESERVE REQUIREMENT (10%)                                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ASSETS                          LIABILITIES                        │   │
    │   │  ┌─────────────────────────────┐ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $100              │ │ Deposits: $1000             │   │   │
    │   │  │ Loans: $900                 │ │                             │   │   │
    │   │  └─────────────────────────────┘ └─────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   │  Total Assets: $1000 = Total Liabilities: $1000                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   LOAN CREATES NEW DEPOSIT ($900 to Borrower)                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ASSETS                          LIABILITIES                        │   │
    │   │  ┌─────────────────────────────┐ ┌─────────────────────────────┐   │   │
    │   │  │ Reserves: $100              │ │ Deposits: $1000 (original)  │   │   │
    │   │  │ Loans: $900                 │ │ Deposits: $900 (new)        │   │   │
    │   │  └─────────────────────────────┘ └─────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   │  Total Assets: $1000 + $900 = $1900                               │   │
    │   │  Total Liabilities: $1000 + $900 = $1900                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   KEY INSIGHT: Loan created new deposit, expanding both sides            │
    │   of the balance sheet. New money was created.                           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Money Creation Process

### Complete Money Creation Chain

The process of money creation through fractional reserve banking follows a sequential chain as loans are deposited, re-lent, and re-deposited across the banking system.

```
COMPLETE MONEY CREATION CHAIN

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Initial Deposit: $1000                                                   │
    │   Reserve Requirement: 10%                                                 │
    │                                                                             │
    │   STEP 1: Bank A receives deposit                                          │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A                                                              │   │
    │   │  Deposits: +$1000                                                   │   │
    │   │  Reserves: +$100 (10% held)                                         │   │
    │   │  Loan: +$900 (90% lent out)                                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        │ $900 loan to Borrower A                                          │
    │        ▼                                                                   │
    │   STEP 2: Borrower A spends $900 with Merchant B                          │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 3: Merchant B deposits $900 in Bank B                              │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank B                                                              │   │
    │   │  Deposits: +$900                                                    │   │
    │   │  Reserves: +$90 (10% held)                                          │   │
    │   │  Loan: +$810 (90% lent out)                                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        │ $810 loan to Borrower C                                          │
    │        ▼                                                                   │
    │   STEP 4: Borrower C spends $810 with Merchant D                          │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 5: Merchant D deposits $810 in Bank C                              │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank C                                                              │   │
    │   │  Deposits: +$810                                                    │   │
    │   │  Reserves: +$81 (10% held)                                          │   │
    │   │  Loan: +$729 (90% lent out)                                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        │ Process continues...                                             │
    │        ▼                                                                   │
    │                                                                             │
    │   CUMULATIVE EFFECT:                                                       │
    │                                                                             │
    │   Round    │ New Deposit     │ New Reserve    │ New Loan                   │
    │   ─────────│─────────────────│────────────────│───────────────────────────│
    │   1        │ $1000.00        │ $100.00        │ $900.00                    │
    │   2        │ $900.00         │ $90.00         │ $810.00                    │
    │   3        │ $810.00         │ $81.00         │ $729.00                    │
    │   4        │ $729.00         │ $72.90         │ $656.10                    │
    │   5        │ $656.10         │ $65.61         │ $590.49                    │
    │   6        │ $590.49         │ $59.05         │ $531.44                    │
    │   7        │ $531.44         │ $53.14         │ $478.30                    │
    │   8        │ $478.30         │ $47.83         │ $430.47                    │
    │   9        │ $430.47         │ $43.05         │ $387.42                    │
    │   10       │ $387.42         │ $38.74         │ $348.68                    │
    │   ...      │ ...             │ ...            │ ...                        │
    │   ─────────│─────────────────│────────────────│───────────────────────────│
    │   TOTAL    │ $10,000.00      │ $1,000.00      │ $9,000.00                  │
    │                                                                             │
    │   Initial deposit of $1000 created $10,000 in total deposits              │
    │   (10x multiplier)                                                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Money Multiplier Formula

The money multiplier expresses the maximum potential increase in the money supply resulting from an initial deposit, given a reserve requirement ratio.

How it works: Simple money multiplier = 1 / Reserve Requirement Ratio. If reserves are 10%, multiplier = 1 / 0.10 = 10. Total money creation = Initial Deposit × Multiplier = $1000 × 10 = $10,000.

However, the actual multiplier is usually smaller due to:

Currency drain: When borrowers or depositors hold some money as cash rather than depositing it

Excess reserves: Banks may hold more than the required minimum

Leakage: Money leaving the banking system

```
MONEY MULTIPLIER FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   SIMPLE MONEY MULTIPLIER (No leakages):                                   │
    │                                                                             │
    │   m = 1 / rr                                                               │
    │                                                                             │
    │   Where:                                                                   │
    │   m = money multiplier                                                     │
    │   rr = reserve requirement ratio (as decimal)                              │
    │                                                                             │
    │   Example: rr = 0.10 → m = 1 / 0.10 = 10                                   │
    │                                                                             │
    │                                                                             │
    │   COMPLEX MONEY MULTIPLIER (With leakages):                                │
    │                                                                             │
    │   m = (1 + c) / (rr + c + e)                                               │
    │                                                                             │
    │   Where:                                                                   │
    │   c = currency drain ratio (cash held by public / deposits)                │
    │   e = excess reserve ratio (excess reserves / deposits)                    │
    │   rr = required reserve ratio                                              │
    │                                                                             │
    │   Example: c = 0.05, e = 0.01, rr = 0.10                                   │
    │   m = (1 + 0.05) / (0.10 + 0.05 + 0.01) = 1.05 / 0.16 = 6.56               │
    │                                                                             │
    │   Real-world multiplier is typically 3-8, not the simple 10               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Reserve Requirements Across Jurisdictions

### Current Reserve Requirement Practices

Reserve requirements vary significantly across countries. Many developed economies have reduced or eliminated reserve requirements entirely, relying instead on interest on reserves as the primary monetary policy tool.

```
RESERVE REQUIREMENTS BY COUNTRY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Country / Region   │ Reserve Requirement   │ Current Status               │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   United States      │ 0%                    │ Eliminated March 2020       │
    │   (Federal Reserve)  │                       │ (previously 10% for large   │
    │                      │                       │  banks)                      │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   Eurozone (ECB)     │ 1%                    │ Reduced from 2%             │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   United Kingdom     │ 0%                    │ No reserve requirements     │
    │   (Bank of England)  │                       │ since 1980s                  │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   Japan (BOJ)        │ 0.05-1.2%             │ Tiered based on deposit     │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   China (PBOC)       │ 5-11%                 │ Variable by bank size and   │
    │                      │                       │ financial stability         │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   India (RBI)        │ 4.5%                  │ Cash Reserve Ratio (CRR)    │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   Brazil             │ 21%                   │ High by international       │
    │                      │                       │ standards                    │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   Canada             │ 0%                    │ No reserve requirements     │
    │   ───────────────────│───────────────────────│─────────────────────────────│
    │   Australia          │ 0%                    │ No reserve requirements     │
    │   (RBA)              │                       │                             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### How Reserve Requirements Have Evolved

Historically, reserve requirements were the primary tool for controlling money supply. Banks were required to hold physical cash equal to a percentage of deposits. Today, most developed central banks use interest on reserves as their main policy tool.

How it works: When reserve requirements are positive, banks must hold non-interest-bearing reserves at the central bank. This acts as a tax on banking, encouraging banks to minimize reserves. Many central banks have lowered requirements to zero and instead pay interest on all reserves. This allows them to control the policy rate without distorting bank behavior.

## Bank Runs and Liquidity Risk

### The Mechanics of a Bank Run

A bank run occurs when a large number of depositors simultaneously withdraw their deposits because they fear the bank will become insolvent. Because banks operate on fractional reserves, they cannot honor all withdrawal requests at once.

How it works: A bank has $100 million in deposits but only $10 million in reserves (10% reserve ratio). If 20% of depositors demand their money back, the bank would need $20 million but only has $10 million in reserves. The bank may be forced to sell loans or borrow, but if the run continues, it becomes insolvent.

```
BANK RUN MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   NORMAL CONDITIONS                                                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  BANK BALANCE SHEET                                                  │   │
    │   │                                                                     │   │
    │   │  ASSETS                    LIABILITIES                              │   │
    │   │  ┌─────────────────────┐   ┌─────────────────────────────────────┐ │   │
    │   │  │ Reserves: $10M      │   │ Deposits: $100M                     │ │   │
    │   │  │ Loans: $90M         │   │ Capital: $10M (equity)              │ │   │
    │   │  └─────────────────────┘   └─────────────────────────────────────┘ │   │
    │   │                                                                     │   │
    │   │  10% reserve ratio: $10M reserves against $100M deposits           │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RUMOR OR SHOCK TRIGGERS FEAR                                             │
    │        │                                                                   │
    │        ▼                                                                   │
    │   DEPOSITORS RUSH TO WITHDRAW                                              │
    │        │                                                                   │
    │        ▼                                                                   │
    │   FIRST WAVE: Bank pays from reserves                                     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   RESERVES DEPLETED: Bank must sell loans at loss                         │
    │        │                                                                   │
    │        ▼                                                                   │
    │   FIRE SALE OF ASSETS: Loan values fall                                   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   CAPITAL DEPLETED: Bank becomes insolvent                                │
    │        │                                                                   │
    │        ▼                                                                   │
    │   BANK FAILURE                                                             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Contagion and Systemic Risk

Bank runs can spread from one bank to another through interconnected financial relationships. This is systemic risk.

How it works: Bank A fails, causing losses to Bank B that held deposits at Bank A. Bank B's depositors, seeing Bank B's losses, withdraw their deposits. Bank B fails, causing losses to Bank C. The chain continues. During the Great Depression, over 9,000 US banks failed between 1930 and 1933 due to contagion.

## Safeguards Against Runs

### Deposit Insurance

Deposit insurance guarantees that depositors will be repaid up to a certain limit even if their bank fails. This eliminates the incentive for runs.

How it works: A government agency (FDIC in US, FSCS in UK, CDIC in Canada) insures deposits up to a limit (typically $250,000 in US, £85,000 in UK). If a bank fails, the insurance agency pays depositors directly. Because depositors know their money is safe, they have no reason to run. Deposit insurance has virtually eliminated bank runs in developed economies since its widespread adoption in the 1930s-1980s.

```
DEPOSIT INSURANCE SCHEMES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Country        │ Scheme Name      │ Coverage Limit   │ Year Established   │
    │   ───────────────│──────────────────│──────────────────│────────────────────│
    │   United States  │ FDIC             │ $250,000         │ 1933               │
    │   ───────────────│──────────────────│──────────────────│────────────────────│
    │   United Kingdom │ FSCS             │ £85,000          │ 2001               │
    │   ───────────────│──────────────────│──────────────────│────────────────────│
    │   Canada         │ CDIC             │ CAD 100,000      │ 1967               │
    │   ───────────────│──────────────────│──────────────────│────────────────────│
    │   Eurozone       │ Various national │ €100,000         │ Various (2008+)    │
    │                  │ (DGS)            │ (harmonized)     │                    │
    │   ───────────────│──────────────────│──────────────────│────────────────────│
    │   Japan          │ DICJ             │ JPY 10 million   │ 1971               │
    │   ───────────────│──────────────────│──────────────────│────────────────────│
    │   Australia      │ FCS              │ AUD 250,000      │ 2008               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Lender of Last Resort

The central bank acts as lender of last resort to solvent but illiquid banks, providing emergency liquidity to prevent runs from forcing unnecessary closures.

How it works: A bank experiencing a run can borrow from the central bank's discount window using its loan portfolio as collateral. This provides the cash needed to meet withdrawal demands until the panic subsides. Bagehot's principle: "Lend freely at a penalty rate against good collateral." The bank remains solvent (assets exceed liabilities) but was temporarily illiquid (could not convert assets to cash fast enough). The central bank loan bridges this gap.

### Capital Requirements

Capital requirements force banks to hold a buffer of equity (shareholder funds) that absorbs losses before depositors are affected.

How it works: If a bank has $10 million in capital and $100 million in deposits, it can lose up to $10 million on its loans before depositors lose anything. Higher capital requirements make banks more resilient to losses. The Basel framework sets international standards (Basel III requires minimum 4.5% Common Equity Tier 1 capital).

```
CAPITAL REQUIREMENTS HIERARCHY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FIRST LOSS: EQUITY (Shareholder Capital)                                 │
    │   ├── Common Equity Tier 1 (CET1): 4.5% minimum                           │
    │   ├── Additional Tier 1: 1.5%                                              │
    │   └── Tier 2: 2.0%                                                         │
    │        │                                                                   │
    │        │ Losses absorbed here first                                        │
    │        ▼                                                                   │
    │   SECOND LOSS: DEPOSIT INSURANCE                                           │
    │   ├── Covers depositors up to limit                                        │
    │   └── Funded by bank premiums                                              │
    │        │                                                                   │
    │        │ If losses exceed capital and insurance...                         │
    │        ▼                                                                   │
    │   THIRD LOSS: DEPOSITORS (Uninsured portion)                               │
    │   └── Losses beyond capital and insurance limits                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Criticisms of Fractional Reserve Banking

### Instability Argument

Critics argue that fractional reserve banking is inherently unstable because it creates a maturity mismatch between short-term deposits and long-term loans.

How it works: Deposits are demandable on short notice (overnight). Loans are made for long periods (years). Under normal conditions, only a small fraction of depositors withdraw at once. But during a panic, the mismatch becomes critical. Full reserve banking would eliminate this mismatch.

### Money Creation Controversy

Critics argue that private banks should not have the power to create money through lending.

How it works: When a bank makes a loan, it creates a new deposit that did not exist before. This expands the money supply without any corresponding increase in real wealth. Critics (including the Chicago Plan of the 1930s, modern Sovereign Money advocates) argue that money creation should be a government monopoly.

### Business Cycle Amplification

Fractional reserve banking may amplify business cycles by expanding credit excessively during booms and contracting sharply during busts.

How it works: During booms, banks become optimistic and lower lending standards, creating excessive money growth and asset bubbles. During busts, banks become pessimistic and call in loans or refuse to roll them over, accelerating the downturn. This is the "credit cycle" or "financial accelerator."

## The Modern Fractional Reserve System

### How Banking Works Today

Modern fractional reserve banking operates with central bank reserves, interest on reserves, and sophisticated risk management.

Current process:

```
MODERN FRACTIONAL RESERVE PROCESS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CENTRAL BANK sets policy rate and pays interest on reserves             │
    │        │                                                                   │
    │        ▼                                                                   │
    │   COMMERCIAL BANKS hold reserves at central bank                          │
    │        │                                                                   │
    │        ├── Required reserves (if any)                                     │
    │        └── Excess reserves (earn interest)                                │
    │        │                                                                   │
    │        ▼                                                                   │
    │   BANKS LEND to creditworthy borrowers                                    │
    │        │                                                                   │
    │        ├── Loans create new deposits (money creation)                     │
    │        ├── Loans are funded by both deposits and bank capital             │
    │        └── Loans are constrained by capital requirements                  │
    │        │                                                                   │
    │        ▼                                                                   │
    │   LOANS ARE SECURITIZED or held to maturity                              │
    │        │                                                                   │
    │        ▼                                                                   │
    │   RISK MANAGEMENT: Diversification, stress testing, hedging              │
    │                                                                             │
    │   DEPOSIT INSURANCE protects retail depositors                            │
    │                                                                             │
    │   SUPERVISION: Regular examinations, stress tests, capital reviews        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Constraints on Bank Lending

Modern banks face multiple constraints that limit money creation:

Capital constraints: Banks must maintain minimum capital ratios. Lending increases risk-weighted assets, requiring more capital.

Liquidity constraints: Banks must maintain sufficient liquid assets to meet potential withdrawals (Liquidity Coverage Ratio under Basel III).

Profitability constraints: Banks will only lend if they can earn a sufficient return above funding costs.

Creditworthy borrowers: Banks cannot create money through loans to non-creditworthy borrowers.

Regulatory constraints: Limits on loan-to-value ratios, debt-to-income ratios, concentration limits.

## Formulas Quick Reference

```
FRACTIONAL RESERVE BANKING FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Reserve Ratio = Reserves / Deposits                                      │
    │                                                                             │
    │   Required Reserves = Reserve Requirement Ratio × Deposits                 │
    │                                                                             │
    │   Excess Reserves = Actual Reserves - Required Reserves                    │
    │                                                                             │
    │   Simple Money Multiplier = 1 / Reserve Requirement Ratio                  │
    │                                                                             │
    │   Total Money Created = Initial Deposit × Money Multiplier                 │
    │                                                                             │
    │   Complex Money Multiplier = (1 + c) / (rr + c + e)                        │
    │   (c = currency drain ratio, e = excess reserve ratio)                     │
    │                                                                             │
    │   Bank Capital Ratio = Capital / Risk-Weighted Assets                      │
    │                                                                             │
    │   Liquidity Coverage Ratio = High-Quality Liquid Assets /                 │
    │                              (Total Net Cash Outflows over 30 days)         │
    │                                                                             │
    │   Net Interest Margin = (Interest Income - Interest Expense) /             │
    │                         Average Earning Assets                              │
    │                                                                             │
    │   Loan Loss Provision = Expected Losses on Loan Portfolio                  │
    │                                                                             │
    │   Deposit Multiplier (with leakage) = ΔDeposits / ΔReserves                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Fractional reserve banking: banks hold only a fraction of deposits as reserves, lending out the remainder.

2. Full reserve banking: 100% reserves, no lending from deposits. Fractional creates money through lending.

3. Reserves: physical cash or central bank deposits. Deposits: bank liabilities to customers.

4. When a bank makes a loan, it creates a new deposit, expanding the money supply.

5. Money multiplier: maximum potential money creation = 1 / reserve requirement ratio.

6. Simple multiplier (10% reserves) = 10. Complex multiplier with leakages = 3-8 typically.

7. Reserve requirements vary globally: US 0%, UK 0%, Eurozone 1%, China 5-11%, Brazil 21%.

8. Bank run occurs when many depositors withdraw simultaneously. Fractional reserves cannot cover all withdrawals.

9. Systemic risk: bank failures spread through interconnected financial system.

10. Deposit insurance (FDIC, FSCS, CDIC) guarantees deposits up to limit, preventing runs.

11. Lender of last resort (central bank) provides emergency liquidity to solvent but illiquid banks.

12. Capital requirements force banks to hold equity buffer. Basel III: 4.5% CET1 minimum.

13. Critics argue fractional reserve banking is unstable, gives banks inappropriate money creation power, and amplifies cycles.

14. Modern constraints on lending: capital requirements, liquidity requirements, profitability, borrower creditworthiness, regulation.

15. Interest on reserves allows central banks to control policy rates even with zero reserve requirements.

16. Deposit insurance + lender of last resort + capital requirements + supervision = safety net against runs.

*This documentation belongs to https://github.com/InterCentury*