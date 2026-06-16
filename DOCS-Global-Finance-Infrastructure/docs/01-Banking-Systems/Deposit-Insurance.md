# Deposit Insurance

## Documentation Overview

Deposit insurance is a system that protects bank depositors from losing their money if a bank fails. It guarantees that depositors will be repaid up to a certain limit, even if the bank becomes insolvent. This document covers the purpose, mechanisms, coverage limits, funding, and history of deposit insurance systems worldwide, with emphasis on the FDIC (United States) as the primary model.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the purpose and function of deposit insurance                  │
    │   Learn how deposit insurance prevents bank runs                            │
    │   Study the FDIC structure and coverage limits                              │
    │   Analyze how deposit insurance is funded (premiums, DIF)                   │
    │   Examine the bank resolution process (payoff vs purchase and assumption)   │
    │   Understand the moral hazard problem and mitigants                         │
    │   Learn deposit insurance systems in other countries                        │
    │   Study historical bank failures and FDIC response                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Purpose

### What is Deposit Insurance

Deposit insurance is a government-backed guarantee that protects depositors' money in the event of a bank failure. If a bank becomes insolvent and cannot return depositors' funds, the deposit insurance agency repays depositors up to a statutory limit.

How it works: A bank pays premiums to the deposit insurance fund. If the bank fails, the insurance agency steps in. It either pays depositors directly (up to the coverage limit) or arranges for another bank to take over the failed bank's deposits. Depositors get their money back within days. The insurance agency then liquidates the failed bank's assets to recover its costs.

```
DEPOSIT INSURANCE MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   NORMAL OPERATIONS                                                         │
    │                                                                             │
    │   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐                   │
    │   │ Depositor   │────►│    Bank     │────►│  Deposit    │                   │
    │   │             │     │             │     │  Insurance  │                   │
    │   │             │◄────│             │     │    Fund     │                   │
    │   └─────────────┘     └─────────────┘     └─────────────┘                   │
    │         │                    │                  │                           │
    │         │                    │                  │                           │
    │         │              Pays premiums      Collects premiums                 │
    │         │              to insurance fund   from banks                       │
    │         │                    │                  │                           │
    │         └────────────────────┴──────────────────┘                           │
    │                                                                             │
    │                                                                             │
    │   BANK FAILURE                                                              │
    │                                                                             │
    │   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐                   │
    │   │ Depositor   │     │   Failed    │     │  Deposit    │                   │
    │   │             │────►│    Bank     │────►│  Insurance  │                   │
    │   │             │     │             │     │    Fund     │                   │
    │   │             │     │ (Insolvent) │     │             │                   │
    │   └─────────────┘     └─────────────┘     └──────┬──────┘                   │
    │         │                                        │                          │
    │         │                                        │ Pays depositors          │
    │         │                                        │ up to coverage limit     │
    │         │                                        ▼                          │
    │         └─────────────────────────────────► ┌─────────────┐                 │
    │                                             │ Depositor   │                 │
    │                                             │  Receives   │                 │
    │                                             │   Payment   │                 │
    │                                             └─────────────┘                 │
    │                                                                             │
    │   OR (Alternative): Purchase and Assumption transaction                     │
    │   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐                   │
    │   │ Depositor   │────►│   Failed    │     │  Healthy    │                   │
    │   │             │     │    Bank     │────►│    Bank     │                   │
    │   │             │     │             │     │ (Acquirer)  │                   │
    │   │             │     └─────────────┘     └─────────────┘                   │
    │   └─────────────┘                               │                           │
    │         │                                       │ Deposits transferred      │
    │         │                                       │ to healthy bank           │
    │         │                                       ▼                           │
    │         └─────────────────────────────────► ┌─────────────┐                 │
    │                                             │ Depositor   │                 │
    │                                             │  Access     │                 │
    │                                             │  Restored   │                 │
    │                                             └─────────────┘                 │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Purpose of Deposit Insurance

Deposit insurance serves multiple critical functions in the financial system.

```
PURPOSES OF DEPOSIT INSURANCE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   PURPOSE 1: PREVENT BANK RUNS                                             │
    │                                                                             │
    │   Without deposit insurance, depositors have incentive to withdraw their   │
    │   money at the first sign of trouble (first mover advantage). This can     │
    │   cause a solvent but illiquid bank to fail. With insurance, depositors    │
    │   know their money is safe even if the bank fails, removing the incentive  │
    │   to run.                                                                  │
    │                                                                             │
    │                                                                             │
    │   PURPOSE 2: PROTECT SMALL DEPOSITORS                                      │
    │                                                                             │
    │   Small depositors (individuals, retirees, small businesses) lack the      │
    │   resources to evaluate bank safety or diversify across banks. Deposit     │
    │   insurance protects their life savings from bank failures.                │
    │                                                                             │
    │                                                                             │
    │   PURPOSE 3: FINANCIAL STABILITY                                           │
    │                                                                             │
    │   By preventing runs, deposit insurance prevents contagion. One bank's     │
    │   failure does not cause depositors at other banks to panic. This keeps    │
    │   the entire banking system stable.                                        │
    │                                                                             │
    │                                                                             │
    │   PURPOSE 4: REDUCE SYSTEMIC RISK                                          │
    │                                                                             │
    │   Large bank failures can trigger financial crises (Lehman Brothers 2008). │
    │   Deposit insurance provides a backstop, reducing systemic risk.           │
    │                                                                             │
    │                                                                             │
    │   PURPOSE 5: MAINTAIN PUBLIC CONFIDENCE                                    │
    │                                                                             │
    │   Public trust in the banking system is essential for economic stability.  │
    │   Deposit insurance assures the public that their money is safe.           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### How Deposit Insurance Prevents Bank Runs

The mechanism by which deposit insurance stops bank runs is based on changing depositor incentives.

```
BANK RUN DYNAMICS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   WITHOUT DEPOSIT INSURANCE                                                │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Rumor of bank trouble                                             │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Depositor A withdraws (first mover advantage)                    │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Depositor B sees line, also withdraws                            │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   More depositors withdraw                                         │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank runs out of reserves                                        │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank fails (even if solvent)                                     │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Other banks face runs (contagion)                                │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   WITH DEPOSIT INSURANCE                                                   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Rumor of bank trouble                                             │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Depositor knows: "My money is insured up to $250,000"            │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   No incentive to withdraw                                         │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   Bank survives (if fundamentally solvent)                         │   │
    │   │        │                                                           │   │
    │   │        ▼                                                           │   │
    │   │   No contagion to other banks                                      │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## FDIC: The US Deposit Insurance System

### History and Establishment

The Federal Deposit Insurance Corporation (FDIC) was created by the Banking Act of 1933 (Glass-Steagall Act) in response to the massive bank failures of the Great Depression.

How it works: Between 1930 and 1933, over 9,000 US banks failed. Depositors lost their savings. Runs were common. President Roosevelt declared a bank holiday (March 1933) to stop the panic. The FDIC was created to restore confidence. When FDIC opened on January 1, 1934, deposits began flowing back into banks. Runs virtually stopped.

```
FDIC HISTORICAL TIMELINE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   1933 ──► Banking Act of 1933 (Glass-Steagall) creates FDIC               │
    │            │                                                                │
    │            ▼                                                                │
    │   1934 ──► FDIC begins operations (January 1)                              │
    │            │ Initial coverage limit: $2,500 (later raised to $5,000 in 1934)│
    │            │                                                                │
    │            ▼                                                                │
    │   1935 ──► Banking Act of 1935 makes FDIC permanent                        │
    │            │                                                                │
    │            ▼                                                                │
    │   1950 ──► Coverage limit raised to $10,000                                │
    │            │                                                                │
    │            ▼                                                                │
    │   1966 ──► Coverage limit raised to $15,000                                │
    │            │                                                                │
    │            ▼                                                                │
    │   1969 ──► Coverage limit raised to $20,000                                │
    │            │                                                                │
    │            ▼                                                                │
    │   1974 ──► Coverage limit raised to $40,000                                │
    │            │                                                                │
    │            ▼                                                                │
    │   1980 ──► Coverage limit raised to $100,000                               │
    │            │                                                                │
    │            ▼                                                                │
    │   2008 ──► Temporary increase to $250,000 (Emergency Economic              │
    │            │ Stabilization Act, during financial crisis)                   │
    │            │                                                                │
    │            ▼                                                                │
    │   2010 ──► Coverage limit made permanent at $250,000 (Dodd-Frank Act)      │
    │            │                                                                │
    │            ▼                                                                │
    │   2024 ──► Coverage remains $250,000 (no inflation adjustment since 2010)  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### FDIC Coverage Limits

The standard coverage limit is $250,000 per depositor, per insured bank, per ownership category.

```
FDIC COVERAGE LIMITS BY OWNERSHIP CATEGORY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   OWNERSHIP CATEGORY                 │ COVERAGE LIMIT                       │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Single Accounts (individual)       │ $250,000 per owner                  │
    │   (owned by one person)              │                                      │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Joint Accounts                     │ $250,000 per co-owner               │
    │   (two or more owners)               │                                      │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Revocable Trust Accounts           │ $250,000 per beneficiary            │
    │   (payable on death, living trusts)  │                                      │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Irrevocable Trust Accounts         │ $250,000 per beneficiary            │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Certain Retirement Accounts        │ $250,000 per owner                  │
    │   (IRA, Keogh, 401(k) if self-       │                                      │
    │   directed, profit sharing)          │                                      │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Employee Benefit Plan Accounts     │ $250,000 per participant            │
    │   (401(k), pension plans)            │                                      │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Corporation, Partnership,          │ $250,000 per entity                 │
    │   Unincorporated Association         │                                      │
    │   ───────────────────────────────────│─────────────────────────────────────│
    │   Government Accounts                │ $250,000 per official custodian     │
    │   (state, county, municipal)         │                                      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### How Coverage Works: Examples

```
COVERAGE EXAMPLES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   EXAMPLE 1: Single individual, one bank                                   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A                                                              │   │
    │   │  ├── Checking: $200,000                                             │   │
    │   │  ├── Savings: $100,000                                              │   │
    │   │  └── CD: $50,000                                                    │   │
    │   │                                                                     │   │
    │   │  Total at same bank: $350,000                                       │   │
    │   │  Insured: $250,000                                                  │   │
    │   │  Uninsured: $100,000                                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE 2: Single individual, two banks                                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A                              │  Bank B                       │   │
    │   │  ├── Checking: $200,000              │  ├── Savings: $150,000        │   │
    │   │  └── Savings: $50,000                │  └── CD: $50,000              │   │
    │   │  Total: $250,000 (fully insured)     │  Total: $200,000 (fully       │   │
    │   │                                       │          insured)             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Key: Different banks = separate coverage limits.                        │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE 3: Joint account (husband and wife)                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A (Joint Account: Husband + Wife)                             │   │
    │   │  ├── Joint checking: $400,000                                       │   │
    │   │  └── Joint savings: $100,000                                        │   │
    │   │                                                                     │   │
    │   │  Total joint: $500,000                                              │   │
    │   │  Each co-owner: $250,000 insured                                    │   │
    │   │  Total insured: $500,000 (fully insured)                           │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   EXAMPLE 4: Multiple ownership categories at same bank                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A                                                              │   │
    │   │  ├── Individual Account: $250,000                                   │   │
    │   │  ├── Joint Account (with spouse): $250,000 (each co-owner)          │   │
    │   │  ├── IRA Account: $250,000                                          │   │
    │   │  └── Trust Account (1 beneficiary): $250,000                        │   │
    │   │                                                                     │   │
    │   │  Total: $1,000,000 (fully insured across 4 ownership categories)   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### What is NOT Covered

FDIC deposit insurance does not cover all financial products.

```
NOT COVERED BY FDIC

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   NOT COVERED                     │ REASON                                  │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   Stocks, bonds, mutual funds     │ These are investments, not deposits.   │
    │                                   │ Value fluctuates with markets.         │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   Annuities                       │ Insurance products, not bank deposits. │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   Life insurance policies         │ Regulated by state insurance depts.    │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   Municipal securities            │ Investments, not deposits.             │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   Safe deposit box contents       │ FDIC insures deposits, not box         │
    │                                   │ contents. Separate insurance needed.   │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   US Treasury bills, bonds, notes │ Backed by US government separately,    │
    │                                   │ not FDIC.                               │
    │   ────────────────────────────────│─────────────────────────────────────────│
    │   Crypto assets                   │ Not considered deposits.               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Deposit Insurance Fund (DIF)

### How the DIF is Funded

The Deposit Insurance Fund is funded by premiums paid by insured banks. The FDIC does not receive taxpayer money.

How it works: Each insured bank pays quarterly assessments based on its total deposits and risk profile. Riskier banks pay higher rates. The funds accumulate in the Deposit Insurance Fund. When a bank fails, the FDIC uses the DIF to pay depositors or to fund the resolution.

```
DIF FUNDING MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ALL INSURED BANKS                                                         │
    │        │                                                                   │
    │        │ Pay quarterly assessments                                         │
    │        │ (Based on domestic deposits × assessment rate)                   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                    DEPOSIT INSURANCE FUND (DIF)                      │   │
    │   │                                                                     │   │
    │   │  Fund balance target: 1.35% - 2.00% of insured deposits            │   │
    │   │  (Designated Reserve Ratio - DRR)                                   │   │
    │   │                                                                     │   │
    │   │  ┌─────────────────────────────────────────────────────────────┐   │   │
    │   │  │  Uses of DIF:                                                │   │   │
    │   │  │  ├── Pay depositors of failed banks                         │   │   │
    │   │  │  ├── Fund purchase and assumption transactions               │   │   │
    │   │  │  ├── Administrative costs of resolutions                     │   │   │
    │   │  │  └── Borrowing repayment (if FDIC borrows from Treasury)    │   │   │
    │   │  └─────────────────────────────────────────────────────────────┘   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        │ If DIF falls below target, FDIC raises assessment rates          │
    │        │ If DIF exceeds target, FDIC may lower rates or pay dividends     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   FDIC ALSO HAS ACCESS TO:                                                │
    │   ├── Treasury line of credit (up to $100 billion)                       │
    │   └── Borrowing from Federal Financing Bank (up to $100 billion)         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Assessment Rates

Banks pay premiums based on their risk. The FDIC uses a risk-based assessment system.

```
RISK-BASED ASSESSMENT SYSTEM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ASSESSMENT RATE DETERMINATION                                             │
    │                                                                             │
    │   Step 1: Assign CAMELS rating (regulatory exam)                            │
    │   ├── C: Capital adequacy                                                   │
    │   ├── A: Asset quality                                                      │
    │   ├── M: Management quality                                                 │
    │   ├── E: Earnings                                                           │
    │   ├── L: Liquidity                                                          │
    │   └── S: Sensitivity to market risk                                         │
    │                                                                             │
    │   Step 2: Assign risk category                                              │
    │   ├── Category I: Large, highly complex banks (separate scorecard)          │
    │   ├── Category II: Higher-risk banks                                        │
    │   ├── Category III: Moderate-risk banks                                     │
    │   └── Category IV: Low-risk banks                                           │
    │                                                                             │
    │   Step 3: Apply assessment rate                                             │
    │                                                                             │
    │   Category I (Scorecard method): 1.5 - 30 basis points                      │
    │   (1 basis point = 0.01%)                                                   │
    │                                                                             │
    │   Example: Bank with $10 billion in domestic deposits                       │
    │   Assessment rate: 5 basis points (0.05%)                                   │
    │   Quarterly assessment: $10B × 0.0005 = $5,000,000                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Bank Resolution Process

### Two Resolution Methods

When a bank fails, the FDIC uses one of two primary resolution methods.

```
RESOLUTION METHODS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   METHOD 1: PURCHASE AND ASSUMPTION (P&A)                                   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Failed Bank ──────────────────────────────────────────┐           │   │
    │   │        │                                                │           │   │
    │   │        │ FDIC arranges sale                             │           │   │
    │   │        ▼                                               ▼            │   │
    │   │   ┌─────────────┐                                 ┌─────────────┐   │   │
    │   │   │  Healthy    │◄────────Deposits transferred────│  Depositors │   │   │
    │   │   │   Bank      │                                 │             │   │   │
    │   │   │ (Acquirer)  │                                 │             │   │   │
    │   │   └─────────────┘                                 └─────────────┘   │   │
    │   │                                                                     │   │
    │   │   FDIC provides financial assistance to acquirer                    │   │
    │   │   Depositors get full access immediately (no disruption)            │   │
    │   │   Failed bank's assets sold to acquirer or liquidated               │   │
    │   │                                                                     │   │
    │   │   90%+ of failures resolved via P&A                                 │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   METHOD 2: PAYOFF (Deposit Insurance Payout)                               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   No healthy bank wants to buy the failed bank                      │   │
    │   │        │                                                            │   │
    │   │        ▼                                                            │   │
    │   │   FDIC takes possession of failed bank's records                    │   │
    │   │        │                                                            │   │
    │   │        ▼                                                            │   │
    │   │   FDIC determines insured deposits for each depositor               │   │
    │   │        │                                                            │   │
    │   │        ▼                                                            │   │
    │   │   FDIC issues checks (up to $250,000 per depositor)                 │   │
    │   │        │                                                            │   │
    │   │        ▼                                                            │   │
    │   │   Depositors receive money within days                              │   │
    │   │        │                                                            │   │
    │   │        ▼                                                            │   │
    │   │   Uninsured depositors receive partial payment (pro rata)           │   │
    │   │   based on asset recovery                                           │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Resolution Process Timeline

When a bank fails, resolution happens over a weekend to minimize disruption.

```
FDIC RESOLUTION WEEKEND

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FRIDAY (Before close)                                                     │
    │   ├── Regulators determine bank is insolvent                                │
    │   ├── State or federal chartering authority closes bank                     │
    │   ├── FDIC appointed as receiver                                            │
    │   └── FDIC teams arrive at bank headquarters                                │
    │        │                                                                    │
    │        ▼                                                                    │
    │   FRIDAY NIGHT (6 PM - Midnight)                                            │
    │   ├── FDIC analyzes bank's books (data extraction)                          │
    │   ├── FDIC solicits bids from healthy banks                                 │
    │   ├── Determine least-cost resolution                                       │
    │   └── Negotiate purchase and assumption agreement (if any)                  │
    │        │                                                                    │
    │        ▼                                                                    │
    │   SATURDAY (Midnight - 12 PM)                                               │
    │   ├── If P&A: Finalize agreement with acquirer                              │
    │   ├── Determine asset valuation and loss sharing                            │
    │   ├── Prepare legal documents                                               │
    │   └── If no buyer: Prepare for payoff                                       │
    │        │                                                                     │
    │        ▼                                                                     │
    │   SATURDAY (12 PM - 6 PM)                                                   │
    │   ├── Calculate insured deposits for each depositor                        │
    │   ├── Prepare depositor notices                                            │
    │   ├── Arrange for checks (if payoff)                                       │
    │   └── Coordinate with acquiring bank systems (if P&A)                      │
    │        │                                                                     │
    │        ▼                                                                     │
    │   SUNDAY (All day)                                                          │
    │   ├── System integration testing (if P&A)                                  │
    │   ├── Train acquiring bank tellers (if P&A)                              │
    │   ├── Mail notices to depositors                                         │
    │   ├── Update FDIC website with instructions                              │
    │   └── Prepare press release                                              │
    │        │                                                                   │
    │        ▼                                                                   │
    │   MONDAY (Opening)                                                        │
    │   ├── If P&A: Failed bank reopens as acquiring bank branch               │
    │   ├── If P&A: Depositors have immediate access                          │
    │   ├── If Payoff: FDIC checks available or mailed                        │
    │   └── No depositor has lost money (up to coverage limit)                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Moral Hazard Problem

### The Risk of Deposit Insurance

Deposit insurance creates moral hazard: banks may take excessive risks because depositors are protected, reducing market discipline.

How it works: Without insurance, depositors monitor bank risk and may withdraw from risky banks (market discipline). With insurance, depositors do not care about bank risk because their money is guaranteed. Banks can take more risks without losing deposits. The FDIC bears the cost if the bank fails.

```
MORAL HAZARD CYCLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DEPOSIT INSURANCE PROTECTS DEPOSITORS                                     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   DEPOSITORS STOP MONITORING BANK RISK                                     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   BANKS TAKE EXCESSIVE RISKS                                               │
    │   ├── Risky loans (higher yield)                                          │
    │   ├── Excessive leverage                                                   │
    │   ├── Concentration in volatile sectors                                   │
    │   └── Weak underwriting standards                                         │
    │        │                                                                   │
    │        ▼                                                                   │
    │   BANKS FAIL MORE FREQUENTLY                                               │
    │        │                                                                   │
    │        ▼                                                                   │
    │   FDIC PAYS HIGHER INSURANCE CLAIMS                                        │
    │        │                                                                   │
    │        ▼                                                                   │
    │   FDIC RAISES ASSESSMENT RATES                                             │
    │        │                                                                   │
    │        ▼                                                                   │
    │   ALL BANKS PAY HIGHER PREMIUMS                                            │
    │   (Safer banks subsidize riskier banks)                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Mitigants to Moral Hazard

The FDIC uses several tools to reduce moral hazard.

```
MORAL HAZARD MITIGANTS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MITIGANT 1: RISK-BASED PREMIUMS                                          │
    │   ├── Riskier banks pay higher assessment rates                           │
    │   ├── Safer banks pay lower rates                                          │
    │   └── Internalizes cost of risk                                            │
    │                                                                             │
    │   MITIGANT 2: COVERAGE LIMIT ($250,000)                                   │
    │   ├── Large depositors still have incentive to monitor                    │
    │   ├── Uninsured depositors ($250k+) can lose money                       │
    │   └── These depositors may withdraw from risky banks                      │
    │                                                                             │
    │   MITIGANT 3: REGULATORY SUPERVISION                                       │
    │   ├── Bank examinations (CAMELS ratings)                                  │
    │   ├── Prompt corrective action (PCA)                                      │
    │   ├── Capital requirements (Basel III)                                    │
    │   └── Enforcement actions for unsafe practices                            │
    │                                                                             │
    │   MITIGANT 4: LEAST-COST RESOLUTION                                        │
    │   ├── FDIC must choose resolution method that costs least                 │
    │   ├── Protects uninsured depositors only if less costly than payout      │
    │   └── Shareholders and unsecured creditors lose value                     │
    │                                                                             │
    │   MITIGANT 5: SYSTEMIC RISK EXCEPTION (Dodd-Frank)                        │
    │   ├── Only allowed with Treasury and Fed approval                         │
    │   ├── Used only to prevent systemic collapse                              │
    │   └── Costs recovered through special assessments on banks                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Notable Bank Failures and FDIC Response

### Key Historical Failures

```
MAJOR BANK FAILURES AND FDIC RESOLUTION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CONTINENTAL ILLINOIS (1984)                                              │
    │   ├── Largest bank failure in US history at the time                       │
    │   ├── Assets: $40 billion                                                  │
    │   ├── Resolution: FDIC took over, protected all depositors (not just       │
    │   │   $100,000 limit) - "too big to fail" precedent                        │
    │   └── Cost to FDIC: $1.8 billion                                          │
    │                                                                             │
    │                                                                             │
    │   SAVINGS AND LOAN CRISIS (1980s-1990s)                                    │
    │   ├── Over 1,000 thrifts failed                                            │
    │   ├── Resolution: FSLIC (thrift insurer) exhausted, replaced by RTC       │
    │   ├── Estimated cost: $160 billion (taxpayer funded)                      │
    │   └── Led to FIRREA Act (1989) restructuring thrift regulation            │
    │                                                                             │
    │                                                                             │
    │   WASHINGTON MUTUAL (2008)                                                 │
    │   ├── Largest bank failure in US history                                   │
    │   ├── Assets: $307 billion                                                 │
    │   ├── Deposits: $188 billion                                               │
    │   ├── Resolution: Purchase and Assumption to JPMorgan Chase               │
    │   ├── No depositor losses                                                  │
    │   └── Shareholders and bondholders wiped out                              │
    │                                                                             │
    │                                                                             │
    │   SILICON VALLEY BANK (2023)                                               │
    │   ├── Assets: $209 billion                                                 │
    │   ├── Deposits: $175 billion                                               │
    │   ├── Failure cause: Bank run triggered by uninsured deposits             │
    │   ├── Resolution: Systemic risk exception invoked                         │
    │   ├── All depositors protected (including uninsured)                      │
    │   └── Cost to DIF: ~$20 billion (recovered via special assessment)        │
    │                                                                             │
    │                                                                             │
    │   SIGNATURE BANK (2023)                                                   │
    │   ├── Assets: $110 billion                                                 │
    │   ├── Failure cause: Contagion from SVB                                   │
    │   ├── Resolution: Systemic risk exception invoked                         │
    │   ├── All depositors protected                                             │
    │   └── Sold to Flagstar Bank (New York Community Bank)                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Deposit Insurance Systems Around the World

### International Comparison

Most countries have deposit insurance systems modeled on the FDIC, with variations in coverage limits.

```
GLOBAL DEPOSIT INSURANCE COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Country / Region   │ System Name      │ Coverage Limit │ Year Est.       │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   United States      │ FDIC             │ $250,000       │ 1933            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Canada             │ CDIC             │ CAD 100,000    │ 1967            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   United Kingdom     │ FSCS             │ £85,000        │ 2001            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Eurozone           │ Various national │ €100,000       │ Various         │
    │                      │ DGS (harmonized) │ (harmonized)   │ (2008+ for many)│
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Japan              │ DICJ             │ JPY 10 million │ 1971            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Australia          │ FCS              │ AUD 250,000    │ 2008            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Germany            │ EdB              │ €100,000       │ 1998            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   France             │ FGDR             │ €100,000       │ 1999            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   China              │ DIC (proposed)   │ RMB 500,000    │ 2015 (pilot)    │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   India              │ DICGC            │ INR 500,000    │ 1962            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Brazil             │ FGC              │ BRL 250,000    │ 1995            │
    │   ───────────────────│──────────────────│────────────────│─────────────────│
    │   Russia             │ DIA              │ RUB 1.4 million│ 2004            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### IADI Principles

The International Association of Deposit Insurers (IADI) sets core principles for effective deposit insurance systems.

```
IADI CORE PRINCIPLES (Abbreviated)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   PRINCIPLE 1: Mandate and objectives clearly defined                      │
    │   PRINCIPLE 2: Legal protection for deposit insurers                        │
    │   PRINCIPLE 3: Independence (operational and financial)                    │
    │   PRINCIPLE 4: Governance structure clear                                   │
    │   PRINCIPLE 5: Member banks required by law to participate                 │
    │   PRINCIPLE 6: Adequate coverage (credible, limited)                       │
    │   PRINCIPLE 7: Reimbursement of depositors within 7 days                   │
    │   PRINCIPLE 8: Public awareness (depositors know coverage)                 │
    │   PRINCIPLE 9: Risk-based premiums (mitigate moral hazard)                 │
    │   PRINCIPLE 10: Access to funding (adequate DIF)                          │
    │   PRINCIPLE 11: Failure resolution authority                               │
    │   PRINCIPLE 12: Coordination with other safety net participants           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
DEPOSIT INSURANCE FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Deposit Insurance Coverage = Min(Deposit Balance, Coverage Limit)        │
    │   Coverage Limit = $250,000 (per depositor, per bank, per ownership        │
    │   category)                                                                │
    │                                                                             │
    │   Total Insured at Bank = Σ(Coverage per ownership category)               │
    │                                                                             │
    │   Uninsured Deposits = Total Deposits - Insured Deposits                   │
    │                                                                             │
    │   Assessment Payment = Domestic Deposits × Assessment Rate                │
    │                                                                             │
    │   Designated Reserve Ratio (DRR) = DIF Balance / Estimated Insured        │
    │   Deposits                                                                 │
    │   Target range: 1.35% - 2.00%                                             │
    │                                                                             │
    │   Loss Given Failure (LGF) = (Deposits + Other Liabilities) - Asset       │
    │   Recovery                                                                 │
    │                                                                             │
    │   Pro Rata Payment to Uninsured Depositors = (Asset Recovery / Total       │
    │   Uninsured Claims) × Individual Uninsured Claim                          │
    │                                                                             │
    │   Deposit Insurance Fund Coverage Ratio = DIF Balance / Insured Deposits   │
    │                                                                             │
    │   Assessment Rate Adjustment = Target Fund Ratio - Actual Fund Ratio       │
    │   (Positive = increase rates, Negative = decrease rates)                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Deposit insurance guarantees depositors will be repaid up to a limit if their bank fails.

2. Primary purpose: prevent bank runs by removing depositor incentive to withdraw.

3. FDIC created in 1933 after over 9,000 banks failed during Great Depression.

4. Standard coverage limit: $250,000 per depositor, per insured bank, per ownership category.

5. Different ownership categories (single, joint, trust, IRA) each have separate $250,000 coverage.

6. Different banks = separate coverage. Can insure more by spreading across banks.

7. Not covered: stocks, bonds, mutual funds, annuities, crypto, safe deposit box contents.

8. Deposit Insurance Fund (DIF) funded by bank premiums, not taxpayer money.

9. Risk-based premiums: riskier banks pay higher assessment rates.

10. Target DIF ratio: 1.35% - 2.00% of insured deposits.

11. Resolution methods: Purchase and Assumption (90%+ of failures) or Payoff.

12. P&A: Healthy bank buys failed bank's deposits. Depositors get immediate access.

13. Payoff: FDIC pays depositors directly (up to $250,000). Takes days to weeks.

14. Resolution weekend: Friday close to Monday opening. No depositor loses insured money.

15. Moral hazard: deposit insurance may encourage excessive bank risk-taking.

16. Mitigants: risk-based premiums, coverage limit, regulation, least-cost resolution.

17. Notable failures: Continental Illinois (1984), S&L Crisis (1980s-90s), WaMu (2008), SVB (2023), Signature (2023).

18. Systemic risk exception (2008, 2023): allows protecting uninsured depositors to prevent contagion.

19. Global systems: CDIC (Canada), FSCS (UK), €100,000 (Eurozone), DICJ (Japan).

20. IADI Core Principles: international standards for deposit insurance systems.

*This documentation belongs to https://github.com/InterCentury*
