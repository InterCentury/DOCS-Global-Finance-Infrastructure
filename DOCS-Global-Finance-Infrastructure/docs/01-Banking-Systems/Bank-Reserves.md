# Bank Reserves

## Documentation Overview

Bank reserves are the portions of customer deposits that banks hold in liquid form rather than lending out. These reserves consist of physical currency held in bank vaults plus deposits held at the central bank. Reserves serve as the ultimate settlement asset in the financial system and are the foundation upon which fractional reserve banking and money creation are built. This document covers the nature, types, purposes, management, and monetary policy implications of bank reserves.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the definition and composition of bank reserves                │
    │   Learn the distinction between required and excess reserves                │
    │   Study the role of reserves in payment settlement                          │
    │   Analyze reserve requirements and their purpose                            │
    │   Examine how reserves are created and destroyed                            │
    │   Understand reserves as the monetary base                                  │
    │   Learn reserve management by commercial banks                              │
    │   Study the evolution from scarce to ample reserves                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Composition

### What are Bank Reserves

Bank reserves are the liquid assets that banks hold to meet withdrawal demands, process payments, and satisfy regulatory requirements. Reserves are the most liquid assets on a bank's balance sheet and represent claims on the central bank.

How it works: When a customer deposits cash, the bank adds to its vault cash. When a bank receives a wire transfer from another bank, its reserve account at the central bank increases. These reserves are instantly available for withdrawal or payment. Banks cannot lend out their reserves; they are held for liquidity and settlement purposes.

```
RESERVE COMPOSITION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TOTAL BANK RESERVES = Vault Cash + Deposits at Central Bank               │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   VAULT CASH                                                        │   │
    │   │   ├── Physical currency (banknotes and coins) held in bank premises │   │
    │   │   ├── ATM cash inventories                                          │   │
    │   │   ├── Cash in transit (being moved between branches)                │   │
    │   │   └── Typically 20-40% of total reserves                            │   │
    │   │                                                                     │   │
    │   │   DEPOSITS AT CENTRAL BANK                                          │   │
    │   │   ├── Digital account balance at central bank                       │   │
    │   │   ├── Used for interbank settlement                                 │   │
    │   │   ├── Can be transferred instantly to other banks                   │   │
    │   │   ├── Earns interest (in most jurisdictions)                        │   │
    │   │   └── Typically 60-80% of total reserves                            │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Required vs Excess Reserves

Reserves are divided into two categories: required reserves (minimum mandated by regulation) and excess reserves (any amount above the requirement).

```
REQUIRED VS EXCESS RESERVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   REQUIRED RESERVES                                                         │
    │   ├── Minimum amount of reserves bank must hold                             │
    │   ├── Calculated as: Reserve Requirement Ratio × Qualifying Deposits        │
    │   ├── Cannot be lent out                                                    │
    │   ├── May earn interest (in many countries)                                 │
    │   └── Violation results in penalties                                        │
    │                                                                             │
    │   EXCESS RESERVES                                                           │
    │   ├── Any reserves above the required amount                                │
    │   ├── Can be lent out to customers or other banks                           │
    │   ├── Can be used to purchase securities                                    │
    │   ├── Earns interest (often same rate as required reserves)                 │
    │   └── Represents potential lending capacity                                 │
    │                                                                             │
    │                                                                             │
    │   RELATIONSHIP:                                                             │
    │                                                                             │
    │   Total Reserves = Required Reserves + Excess Reserves                      │
    │                                                                             │
    │   Excess Reserves = Total Reserves - Required Reserves                      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Reserve Requirement Ratio

The reserve requirement ratio is the fraction of customer deposits that banks must hold as reserves. This ratio determines the theoretical maximum money multiplier.

How it works: If the reserve requirement is 10%, a bank with $100 million in deposits must hold at least $10 million in reserves. The remaining $90 million can be lent out. The reserve requirement is a tool of monetary policy, though many countries have reduced or eliminated it.

```
RESERVE REQUIREMENT CALCULATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FORMULA: Required Reserves = Reserve Requirement Ratio × Deposits         │
    │                                                                             │
    │   EXAMPLE 1 (10% requirement):                                              │
    │   Deposits = $100,000,000                                                   │
    │   Required Reserves = 0.10 × $100,000,000 = $10,000,000                     │
    │                                                                             │
    │   EXAMPLE 2 (5% requirement):                                               │
    │   Deposits = $100,000,000                                                   │
    │   Required Reserves = 0.05 × $100,000,000 = $5,000,000                      │
    │                                                                             │
    │   EXAMPLE 3 (0% requirement):                                               │
    │   Deposits = $100,000,000                                                   │
    │   Required Reserves = 0 × $100,000,000 = $0                                 │
    │   (All reserves are excess)                                                 │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## The Role of Reserves

### Settlement Asset

Reserves are the ultimate settlement asset in the financial system. When one bank pays another, reserves transfer between their central bank accounts.

How it works: Bank A owes Bank B $1 million. Bank A's central bank reserve account is debited $1 million. Bank B's central bank reserve account is credited $1 million. The payment is final and irrevocable. No other asset can settle interbank obligations with zero credit risk.

```
RESERVE SETTLEMENT MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BEFORE SETTLEMENT:                                                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK LEDGER                                                │   │
    │   │  ├── Bank A Reserve Account: $10,000,000                            │   │
    │   │  └── Bank B Reserve Account: $5,000,000                             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   BANK A PAYS $1,000,000 TO BANK B                                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK LEDGER                                                │   │
    │   │  ├── Bank A Reserve Account: $10,000,000 - $1,000,000 = $9,000,000  │   │
    │   │  └── Bank B Reserve Account: $5,000,000 + $1,000,000 = $6,000,000   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   AFTER SETTLEMENT:                                                         │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK LEDGER                                                │   │
    │   │  ├── Bank A Reserve Account: $9,000,000                             │   │
    │   │  └── Bank B Reserve Account: $6,000,000                             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Key insight: Only central bank reserves can settle interbank payments     │
    │   with finality and no credit risk.                                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Liquidity Buffer

Reserves serve as a liquidity buffer to meet depositor withdrawals and payment obligations. Banks cannot predict exactly when depositors will withdraw cash or when payments will be due.

How it works: If too many depositors withdraw at once, the bank uses its reserves. If reserves are insufficient, the bank must borrow (from other banks, the discount window, or the federal funds market). Larger reserves mean greater ability to withstand unexpected outflows.

### Prudential Requirement

Reserve requirements are a prudential tool to ensure banks maintain adequate liquidity. By forcing banks to hold a minimum percentage of deposits as reserves, regulators reduce the risk of bank runs.

How it works: Even if all depositors demanded their money simultaneously, reserves alone would not be sufficient (fractional reserve). But reserve requirements ensure banks have enough liquid assets to meet normal withdrawal patterns. Combined with deposit insurance and lender of last resort, reserves contribute to financial stability.

## Reserves and the Monetary Base

### Monetary Base Definition

The monetary base (also called M0, high-powered money, or base money) consists of currency in circulation plus bank reserves. It is the foundation upon which the broader money supply is built.

```
MONETARY BASE COMPOSITION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MONETARY BASE (M0) = Currency in Circulation + Bank Reserves              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   CURRENCY IN CIRCULATION                                           │   │
    │   │   ├── Physical money held by the public (individuals, businesses)   │   │
    │   │   ├── Not held by banks                                             │   │
    │   │   └── Approximately 90-95% of all physical currency                 │   │
    │   │                                                                     │   │
    │   │   BANK RESERVES                                                     │   │
    │   │   ├── Vault cash (physical currency held by banks)                  │   │
    │   │   ├── Deposits at central bank (digital reserves)                   │   │
    │   │   └── Approximately 5-10% of physical currency + digital balances   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RELATIONSHIP TO MONEY SUPPLY:                                             │
    │                                                                             │
    │   M1 (Narrow Money) = Monetary Base × Money Multiplier                      │
    │                                                                             │
    │   The money multiplier (typically 3-8) determines how much M1 is created    │
    │   from a given monetary base through fractional reserve banking.            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Monetary Base vs Money Supply

```
COMPARISON: MONETARY BASE VS MONEY SUPPLY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   Aspect                  │ Monetary Base (M0)  │ Money Supply (M1/M2)      │
    │   ────────────────────────│─────────────────────│────────────────────────── │
    │   Components              │ Currency +          │ M0 + demand deposits +    │
    │                           │ bank reserves       │ other checkable deposits  │
    │   ────────────────────────│─────────────────────│────────────────────────── │
    │   Created by              │ Central bank only   │ Central bank +            │
    │                           │                     │ commercial banks          │
    │   ────────────────────────│─────────────────────│────────────────────────── │
    │   Credit risk             │ None (central       │ Yes (bank could fail)     │
    │                           │ bank liability)     │                           │
    │   ────────────────────────│─────────────────────│────────────────────────── │
    │   Size (US, 2024)         │ ~$6 trillion        │ M2: ~$20 trillion         │
    │   ────────────────────────│─────────────────────│────────────────────────── │
    │   Controllability by      │ Direct (open market │ Indirect (through         │
    │   central bank            │ operations)         │ multiplier)               │
    │   ────────────────────────│─────────────────────│────────────────────────── │
    │   Role                    │ Foundation of       │ Medium of exchange for    │
    │                           │ monetary system     │ everyday transactions     │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Reserve Creation and Destruction

### How Reserves are Created

Reserves are created when the central bank expands its balance sheet, primarily through open market purchases or lending to banks.

```
RESERVE CREATION MECHANISMS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MECHANISM 1: Open Market Purchase                                         │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ──────$100 million─────────────────► COMMERCIAL BANK  │   │
    │   │                     (payment for bonds)                             │   │
    │   │                                                                     │   │
    │   │  CENTRAL BANK ◄─────Government Bonds───────────── COMMERCIAL BANK   │   │
    │   │                                                                     │   │
    │   │  Result: Bank reserves increase by $100 million                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   MECHANISM 2: Discount Window Lending                                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ──────$50 million──────────────────► COMMERCIAL BANK  │   │
    │   │                     (loan to bank)                                  │   │
    │   │                                                                     │   │
    │   │  CENTRAL BANK ◄─────Collateral────────────────── COMMERCIAL BANK    │   │
    │   │                                                                     │   │
    │   │  Result: Bank reserves increase by $50 million                      │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   MECHANISM 3: Quantitative Easing                                          │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ──────Large asset purchases─────────► COMMERCIAL BANK │   │
    │   │                     (bonds, MBS, corporate debt)                    │   │
    │   │                                                                     │   │
    │   │  Result: Massive reserve creation (trillions during crises)         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### How Reserves are Destroyed

Reserves are destroyed when the central bank contracts its balance sheet, primarily through open market sales or loan repayments.

```
RESERVE DESTRUCTION MECHANISMS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MECHANISM 1: Open Market Sale                                             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ◄─────$100 million───────────────── COMMERCIAL BANK   │   │
    │   │                     (payment for bonds)                             │   │
    │   │                                                                     │   │
    │   │  CENTRAL BANK ──────Government Bonds─────────────► COMMERCIAL BANK  │   │
    │   │                                                                     │   │
    │   │  Result: Bank reserves decrease by $100 million                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   MECHANISM 2: Discount Window Repayment                                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ◄─────$50 million────────────────── COMMERCIAL BANK   │   │
    │   │                     (loan repayment)                                │   │
    │   │                                                                     │   │
    │   │  CENTRAL BANK ──────Collateral──────────────────► COMMERCIAL BANK   │   │
    │   │                                                                     │   │
    │   │  Result: Bank reserves decrease by $50 million                      │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   MECHANISM 3: Quantitative Tightening                                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ──────Bonds mature─────────────────► No reinvestment  │   │
    │   │                     (or sells assets)                               │   │
    │   │                                                                     │   │
    │   │  Result: Reserves decrease as assets leave balance sheet            │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Reserve Management by Banks

### Daily Reserve Management

Banks must manage their reserves daily to meet requirements and avoid overdrafts. This is one of the most critical daily treasury functions.

How it works: At the start of each day, the bank calculates its required reserves based on deposit levels. It then forecasts net payment flows (incoming vs outgoing wires, check clearing, etc.). It monitors its actual reserve balance throughout the day. If projected to be below requirement, it borrows reserves (fed funds market, discount window). If above, it lends excess reserves to other banks.

```
DAILY RESERVE MANAGEMENT PROCESS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STEP 1: Calculate Reserve Requirement                                     │
    │   ├── Based on average deposits over prior period (lagged accounting)       │
    │   └── Required = RR Ratio × Qualifying Deposits                             │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 2: Forecast Reserve Position                                         │
    │   ├── Project incoming payments (customer deposits, wire receipts)          │
    │   ├── Project outgoing payments (withdrawals, wire payments)                │
    │   ├── Forecast net change                                                   │
    │   └── Calculate projected end-of-day balance                                │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 3: Identify Shortfall or Surplus                                     │
    │        │                                                                    │
    │        ├─────────────────────────────────────────────────────┐              │
    │        ▼                                                     ▼              │
    │   IF SHORTFALL                                          IF SURPLUS          │
    │   ├── Borrow from fed funds market                   ├── Lend in fed        │
    │   ├── Borrow from discount window                    │   funds market       │
    │   ├── Sell securities (repos)                        ├── Buy securities     │
    │   ├── Reduce lending                                 │   (reverse repo)     │
    │   └── Attract new deposits                           └── Reduce             │
    │                                                          borrowings         │
    │        │                                                     │              │
    │        └──────────────────────┬──────────────────────────────┘              │
    │                               │                                             │
    │                               ▼                                             │
    │   STEP 4: Execute Trades in Reserve Market                                  │
    │                                                                             │
    │   STEP 5: Monitor and Adjust Throughout Day                                 │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Federal Funds Market

The federal funds market is where banks lend excess reserves to other banks overnight. The interest rate on these loans is the federal funds rate, the primary policy target of the Federal Reserve.

How it works: A bank with excess reserves (surplus) lends to a bank with a reserve shortfall (deficit). The loan is unsecured and overnight. The interest rate is negotiated between the two banks but stays near the central bank's target. The central bank influences this rate through open market operations and interest on reserves.

```
FEDERAL FUNDS MARKET MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BANK WITH EXCESS RESERVES              BANK WITH RESERVE SHORTFALL        │
    │   (Surplus)                              (Deficit)                          │
    │                                                                             │
    │   ┌─────────────────────────┐            ┌─────────────────────────┐        │
    │   │ Bank A                  │            │ Bank B                  │        │
    │   │ Reserve Balance: $150M  │            │ Reserve Balance: $40M   │        │
    │   │ Required Reserves: $100M│            │ Required Reserves: $50M │        │
    │   │ Excess Reserves: $50M   │            │ Reserve Shortfall: $10M │        │
    │   └───────────┬─────────────┘            └───────────┬─────────────┘        │
    │               │                                      │                      │
    │               │         $10 million loan             │                      │
    │               │         at 5.25% interest            │                      │
    │               └──────────────────────────────────────┘                      │
    │                                                                             │
    │                                                                             │
    │   AFTER LOAN:                                                               │
    │                                                                             │
    │   Bank A Reserves: $150M - $10M = $140M (Excess reduces to $40M)            │
    │   Bank B Reserves: $40M + $10M = $50M (Shortfall eliminated)                │
    │                                                                             │
    │   Next day: Loan repaid with interest.                                      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Reserve Maintenance Period

Reserve requirements are calculated over a maintenance period (typically two weeks), not daily. This gives banks flexibility in managing reserves.

How it works: The bank's reserves are averaged over the maintenance period. As long as the average meets the requirement, the bank can have daily deficits as long as they are offset by surpluses on other days. This reduces the cost of reserve management.

```
RESERVE MAINTENANCE PERIOD EXAMPLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Maintenance Period: 14 days                                               │
    │   Required Average Reserves: $100 million per day                           │
    │                                                                             │
    │   Day │ Actual Reserves ($M) │ Above/Below Requirement                      │
    │   ────│──────────────────────│───────────────────────────────────────────── │
    │   1   │ 110                  │ +10                                          │
    │   2   │ 105                  │ +5                                           │
    │   3   │ 95                   │ -5                                           │
    │   4   │ 90                   │ -10                                          │
    │   5   │ 100                  │ 0                                            │
    │   6   │ 95                   │ -5                                           │
    │   7   │ 115                  │ +15                                          │
    │   8   │ 100                  │ 0                                            │
    │   9   │ 85                   │ -15                                          │
    │   10  │ 110                  │ +10                                          │
    │   11  │ 100                  │ 0                                            │
    │   12  │ 95                   │ -5                                           │
    │   13  │ 105                  │ +5                                           │
    │   14  │ 100                  │ 0                                            │
    │                                                                             │
    │   Total Above: +45                                                          │
    │   Total Below: -40                                                          │
    │   Net Average: (14 × $100M + $5M) / 14 = $100.36M (Requirement met)         │
    │                                                                             │
    │   Key insight: Banks can have daily deficits as long as total               │
    │   average meets requirement over the full period.                           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Interest on Reserves

### IORB (Interest on Reserve Balances)

Most major central banks pay interest on reserves. This allows them to set a floor under short-term interest rates and implement monetary policy even with abundant reserves.

How it works: The central bank announces an interest rate paid on bank reserves (IORB rate). Banks will not lend reserves to other banks for less than the IORB rate, because they can simply hold reserves and earn IORB. This creates a floor (lower bound) for the federal funds rate. The central bank can then set the policy rate by adjusting IORB.

```
INTEREST ON RESERVES MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CENTRAL BANK SETS IORB RATE = 5.00%                                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Bank A has $100 million excess reserves                            │   │
    │   │                                                                     │   │
    │   │  OPTION 1: Hold reserves at central bank                            │   │
    │   │  └── Earns 5.00% interest (risk-free)                               │   │
    │   │                                                                     │   │
    │   │  OPTION 2: Lend to Bank B in fed funds market                       │   │
    │   │  └── Bank B will pay at most 5.00% (otherwise Bank A prefers        │   │
    │   │      holding reserves)                                              │   │
    │   │                                                                     │   │
    │   │  OPTION 3: Lend to a corporate customer                             │   │
    │   │  └── Must earn above 5.00% to be worthwhile after risk premium      │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RESULT:                                                                  │
    │   ├── Federal funds rate cannot fall below IORB rate                      │
    │   ├── IORB rate becomes the effective floor for short-term rates         │
    │   ├── Central bank controls rates without needing to actively manage     │
    │   │   reserve scarcity                                                   │
    │   └── Enables ample reserves regime (post-2008)                           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### ON RRP (Overnight Reverse Repo Facility)

The overnight reverse repo facility provides an additional floor for interest rates, available to a broader set of financial institutions (money market funds, government-sponsored enterprises, not just banks).

How it works: Eligible institutions can lend cash to the central bank overnight in exchange for Treasury securities, earning the ON RRP rate. This provides a risk-free investment option, setting a floor under short-term rates for non-bank institutions.

## Scarce Reserves vs Ample Reserves

### Historical Evolution

The reserve regime has changed dramatically over time. Before 2008, reserves were scarce. After 2008, reserves became abundant.

```
SCARCE VS AMPLE RESERVES COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Feature              │ Scarce Reserves         │ Ample Reserves          │
    │                        │ (Pre-2008)              │ (Post-2008)             │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Reserve level        │ Near minimum required   │ Vastly above required   │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Typical total        │ ~$50 billion            │ ~$3 trillion+           │
    │   reserves (US)        │                         │                         │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Reserve scarcity     │ High                    │ None                     │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Fed funds rate       │ Sensitive to small      │ Stable, held at IORB    │
    │   behavior             │ reserve changes         │ floor                    │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Monetary policy      │ Open market operations  │ Interest on reserves    │
    │   implementation       │ (scarce reserves        │ (ample reserves         │
    │                        │ framework)              │ framework)              │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Open market          │ Frequent (daily)        │ Rare (only to maintain  │
    │   operations           │                         │ ample level)            │
    │   ─────────────────────│─────────────────────────│─────────────────────────│
    │   Period               │ Pre-2008, pre-COVID     │ 2008-present (with      │
    │                        │                         │ QE episodes)            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Scarce Reserves Framework (Pre-2008)

In the scarce reserves framework, the central bank actively managed the quantity of reserves to hit its interest rate target.

How it worked: The central bank kept reserves just above the minimum required level. Small changes in reserve supply caused noticeable changes in the federal funds rate. The central bank used daily open market operations to add or remove small amounts of reserves to keep the rate at target.

### Ample Reserves Framework (Post-2008)

In the ample reserves framework, the central bank supplies far more reserves than banks need to meet requirements. Interest on reserves becomes the primary policy tool.

How it works: The central bank sets the IORB rate. Banks have no incentive to lend reserves for less than IORB, so market rates stay at or above IORB. Open market operations are not needed for daily rate control. The central bank only intervenes to maintain the ample level if reserves fall too low.

## Reserves and the Money Multiplier

### The Traditional Money Multiplier

The money multiplier describes how an initial reserve injection can lead to a larger increase in the money supply through fractional reserve lending.

```
TRADITIONAL MONEY MULTIPLIER

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   SIMPLE MODEL (No leakages):                                              │
    │                                                                             │
    │   Money Multiplier = 1 / Reserve Requirement Ratio                         │
    │                                                                             │
    │   EXAMPLE (RR = 10%):                                                      │
    │   Multiplier = 1 / 0.10 = 10                                              │
    │   $1 billion reserve injection → $10 billion money supply increase        │
    │                                                                             │
    │                                                                             │
    │   COMPLEX MODEL (With leakages):                                           │
    │                                                                             │
    │   Money Multiplier = (1 + c) / (rr + c + e)                                │
    │                                                                             │
    │   Where:                                                                   │
    │   c = currency drain ratio (cash held by public / deposits)               │
    │   e = excess reserve ratio (excess reserves / deposits)                   │
    │   rr = required reserve ratio                                              │
    │                                                                             │
    │   EXAMPLE (c = 0.05, e = 0.01, rr = 0.10):                                │
    │   Multiplier = (1 + 0.05) / (0.10 + 0.05 + 0.01) = 1.05 / 0.16 = 6.56    │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Multiplier in the Ample Reserves Era

The traditional money multiplier has broken down in the ample reserves era. Banks hold vast excess reserves that they do not lend out. Reserve quantity does not constrain lending.

How it works: Banks are capital-constrained, not reserve-constrained. They will only lend if they have profitable opportunities and sufficient capital. Adding more reserves does not force banks to lend. The money multiplier is not a useful predictor in ample reserves regimes.

## Formulas Quick Reference

```
RESERVE FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Total Reserves = Vault Cash + Deposits at Central Bank                   │
    │                                                                             │
    │   Required Reserves = Reserve Requirement Ratio × Qualifying Deposits      │
    │                                                                             │
    │   Excess Reserves = Total Reserves - Required Reserves                     │
    │                                                                             │
    │   Monetary Base (M0) = Currency in Circulation + Bank Reserves             │
    │                                                                             │
    │   Reserve Ratio (actual) = Total Reserves / Total Deposits                 │
    │                                                                             │
    │   Simple Money Multiplier = 1 / Reserve Requirement Ratio                  │
    │                                                                             │
    │   Complex Money Multiplier = (1 + c) / (rr + c + e)                        │
    │                                                                             │
    │   Real Interest Rate on Reserves = IORB Rate - Inflation Rate              │
    │                                                                             │
    │   Federal Funds Rate Target Range = [IORB - Spread, IORB + Spread]        │
    │   (Typically IORB is the floor)                                            │
    │                                                                             │
    │   Reserve Maintenance Average = (Sum of Daily Reserves) / Days in Period   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Bank reserves are vault cash plus deposits at central bank. Most liquid asset on bank balance sheet.

2. Required reserves: minimum mandated by regulation. Calculated as RR ratio × deposits.

3. Excess reserves: any reserves above requirement. Can be lent out.

4. Reserves are the ultimate settlement asset. Interbank payments settle through central bank reserve accounts.

5. Reserves serve as liquidity buffer for withdrawals and payments.

6. Reserve requirements reduce bank run risk (combined with deposit insurance, LOLR).

7. Monetary base (M0) = currency in circulation + bank reserves.

8. Reserves created by central bank through open market purchases, discount window lending, QE.

9. Reserves destroyed by open market sales, loan repayments, QT.

10. Banks manage reserves daily to meet requirements. Fed funds market allows lending/borrowing.

11. Reserve maintenance period (typically 2 weeks) allows averaging, gives flexibility.

12. Interest on reserves (IORB) is paid by central bank. Creates floor under short-term rates.

13. ON RRP facility extends floor to non-bank institutions (money market funds).

14. Scarce reserves framework (pre-2008): central bank actively managed reserve quantity.

15. Ample reserves framework (post-2008): reserves abundant, IORB primary policy tool.

16. Traditional money multiplier: 1 / RR ratio. Has broken down in ample reserves era.

17. In ample reserves, banks are capital-constrained, not reserve-constrained.

18. Excess reserves earn interest. Banks hold them willingly.

19. QE created trillions in excess reserves. Did not cause high inflation (2010s).

20. Reserve management is a core daily treasury function for all commercial banks.

*This documentation belongs to https://github.com/InterCentury*