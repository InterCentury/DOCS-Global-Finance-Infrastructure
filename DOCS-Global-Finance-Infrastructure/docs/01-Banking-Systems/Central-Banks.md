# 03 - Central Banks

## Documentation Overview

Central banks are the apex financial institutions in a country or monetary union, responsible for managing the currency, money supply, and interest rates. They serve as the banker to commercial banks and the government, and act as the lender of last resort. This document covers the functions, tools, balance sheet operations, independence, and international roles of central banks in the modern financial system.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the core functions and mandates of central banks               │
    │   Learn monetary policy objectives and implementation tools                 │
    │   Study central bank balance sheet structure and operations                 │
    │   Analyze the lender of last resort function                                │
    │   Examine payment system oversight and operation                            │
    │   Understand central bank independence and accountability                   │
    │   Learn the role of central banks in financial stability                    │
    │   Study international central bank cooperation                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Core Functions

### What is a Central Bank

A central bank is a public institution that manages a country's currency, money supply, and interest rates. Unlike commercial banks, central banks do not serve the general public. Instead, they serve as banks for commercial banks and the government.

How it works: Commercial banks hold accounts at the central bank, using them to settle payments among themselves. The government maintains its treasury account at the central bank. The central bank controls the creation of base money (currency and bank reserves) and influences the broader money supply through monetary policy.

```
CENTRAL BANK CORE FUNCTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │                       CENTRAL BANK                                  │   │
    │   │                             │                                       │   │
    │   │         ┌───────────────────┼───────────────────┐                   │   │
    │   │         │                   │                   │                   │   │
    │   │         ▼                   ▼                   ▼                   │   │
    │   │   ┌───────────┐       ┌───────────┐       ┌───────────┐             │   │
    │   │   │ Monetary  │       │ Currency  │       │ Banker to │             │   │
    │   │   │ Policy    │       │ Issuance  │       │ Banks     │             │   │
    │   │   └─────┬─────┘       └─────┬─────┘       └─────┬─────┘             │   │
    │   │         │                   │                   │                   │   │
    │   │         └───────────────────┼───────────────────┘                   │   │
    │   │                             │                                       │   │
    │   │         ┌───────────────────┼───────────────────┐                   │   │
    │   │         │                   │                   │                   │   │
    │   │         ▼                   ▼                   ▼                   │   │
    │   │   ┌───────────┐       ┌───────────┐       ┌───────────┐             │   │
    │   │   │Lender of  │       │Payment    │       │Financial  │             │   │
    │   │   │Last Resort│       │Systems    │       │Stability  │             │   │
    │   │   └───────────┘       └───────────┘       └───────────┘             │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   FUNCTION DETAILS:                                                         │
    │                                                                             │
    │   1. Monetary Policy: Sets interest rates and controls money supply         │
    │      to achieve price stability and maximum employment.                     │
    │                                                                             │
    │   2. Currency Issuance: Has sole right to issue banknotes and coins.        │
    │      Maintains public confidence in currency.                               │
    │                                                                             │
    │   3. Banker to Banks: Holds reserve accounts for commercial banks.          │
    │      Provides settlement services for interbank payments.                   │
    │                                                                             │
    │   4. Banker to Government: Manages government's bank account.               │
    │      Processes tax receipts and government payments.                        │
    │                                                                             │
    │   5. Lender of Last Resort: Provides emergency liquidity to solvent         │
    │      but illiquid banks during crises.                                      │
    │                                                                             │
    │   6. Payment Systems Oversight: Operates or oversees RTGS systems.          │
    │      Ensures smooth functioning of national payment infrastructure.         │
    │                                                                             │
    │   7. Financial Stability: Monitors systemic risk. Regulates and             │
    │      supervises systemically important institutions.                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Central Bank Mandates

Different central banks have different statutory mandates defining their primary objectives.

```
CENTRAL BANK MANDATES BY COUNTRY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Central Bank           │ Mandate Type          │ Primary Target           │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   Federal Reserve (US)   │ Dual Mandate          │ 2% inflation +           │
    │                          │                       │ maximum employment       │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   European Central Bank  │ Price Stability       │ Below but close to 2%    │
    │   (Eurozone)             │ (Hierarchical)        │ inflation                │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   Bank of England (UK)   │ Price Stability +     │ 2% inflation target      │
    │                          │ Support growth        │ (symmetric)              │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   Bank of Japan (JP)     │ Price Stability       │ 2% inflation target      │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   People's Bank of China │ Multiple Objectives   │ Price + growth +         │
    │   (CN)                   │                       │ exchange rate stability  │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   Swiss National Bank    │ Price Stability       │ Below 2% inflation       │
    │   (CH)                   │                       │                          │
    │   ───────────────────────│───────────────────────│───────────────────────── │
    │   Reserve Bank of India  │ Price Stability +     │ 4% inflation (±2%)       │
    │   (IN)                   │ Growth                │                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Monetary Policy

### Policy Objectives

Monetary policy is the central bank's primary tool for achieving macroeconomic stability. The main objectives are price stability, maximum employment, and moderate long-term interest rates.

How it works: The central bank adjusts the policy rate (the interest rate it pays on reserves or charges for overnight loans) to influence borrowing costs throughout the economy. Lower rates stimulate spending and inflation. Higher rates cool spending and reduce inflation.

```
MONETARY POLICY OBJECTIVES HIERARCHY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   PRIMARY OBJECTIVE: Price Stability                                        │
    │   │                                                                         │
    │   ├── Most central banks target 2% inflation                                │
    │   ├── Prevents deflation (falling prices)                                   │
    │   ├── Prevents high inflation (eroding savings)                             │
    │   └── Provides anchor for expectations                                      │
    │   │                                                                         │
    │   ▼                                                                         │
    │   SECONDARY OBJECTIVES:                                                     │
    │   │                                                                         │
    │   ├── Maximum employment (Fed dual mandate)                                 │
    │   ├── Financial stability                                                   │
    │   ├── Moderate long-term interest rates                                     │
    │   └── Exchange rate stability (some central banks)                          │
    │   │                                                                         │
    │   ▼                                                                         │
    │   ULTIMATE GOALS:                                                           │
    │   │                                                                         │
    │   ├── Sustainable economic growth                                           │
    │   ├── High employment                                                       │
    │   └── Stable purchasing power of currency                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Monetary Policy Tools

```
MONETARY POLICY TOOLKIT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TOOL                      │ TYPE          │ MECHANISM                     │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Policy Rate               │ Conventional  │ Interest paid on reserves     │
    │   (Interest on Reserves)    │               │ influences all rates          │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Open Market Operations    │ Conventional  │ Buy/sell bonds to adjust      │
    │   (OMO)                     │               │ reserve levels                │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Reserve Requirements      │ Conventional  │ Minimum reserves as %         │
    │                             │               │ of deposits                   │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Discount Window           │ Conventional  │ Lending to banks at           │
    │                             │               │ penalty rate                  │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Quantitative Easing (QE)  │ Unconventional│ Large-scale asset purchases   │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Negative Interest Rates   │ Unconventional│ Charge banks for reserves     │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Forward Guidance          │ Unconventional│ Communication about future    │
    │                             │               │ policy path                   │
    │   ──────────────────────────│───────────────│────────────────────────────── │
    │   Yield Curve Control (YCC) │ Unconventional│ Cap specific bond yields      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Policy Rate Transmission

The policy rate transmits through the financial system to affect borrowing costs for households and businesses.

```
POLICY RATE TRANSMISSION CHAIN

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CENTRAL BANK CHANGES POLICY RATE                                          │
    │        │                                                                    │
    │        ▼                                                                    │
    │   INTERBANK LENDING RATE CHANGES                                            │
    │   (Federal Funds Rate, EONIA, SONIA)                                        │
    │        │                                                                    │
    │        ▼                                                                    │
    │   COMMERCIAL BANK FUNDING COSTS CHANGE                                      │
    │        │                                                                    │
    │        ├─────────────────────────────────────────────────────┐              │
    │        ▼                                                     ▼              │
    │   LENDING RATES CHANGE                                  DEPOSIT RATES       │
    │   (Mortgages, business loans,                          CHANGE               │
    │    credit cards, auto loans)                           (Savings, CDs)       │
    │        │                                                     │              │
    │        ▼                                                     ▼              │
    │   BORROWING COSTS                                      SAVING INCENTIVES    │
    │   FOR HOUSEHOLDS &                                     CHANGE               │
    │   BUSINESSES                                                                │
    │        │                                                     │              │
    │        └──────────────────────┬──────────────────────────────┘              │
    │                               │                                             │
    │                               ▼                                             │
    │                    SPENDING AND INVESTMENT CHANGES                          │
    │                               │                                             │
    │                               ▼                                             │
    │                    AGGREGATE DEMAND CHANGES                                 │
    │                               │                                             │
    │                               ▼                                             │
    │                    INFLATION AND OUTPUT ADJUST                              │
    │                                                                             │
    │   Lag: 12-24 months for full effect                                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Central Bank Balance Sheet

### Structure of the Balance Sheet

The central bank balance sheet is the foundation of the monetary system. Assets (what the central bank owns) are matched by liabilities (what the central bank owes).

```
CENTRAL BANK BALANCE SHEET STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ASSETS                                    LIABILITIES                     │
    │   ───────────────────────────               ───────────────────────────     │
    │                                             │                               │
    │   ┌─────────────────────────────┐           ┌─────────────────────────────┐ │
    │   │ Government Securities       │           │ Currency in Circulation     │ │
    │   │ (Treasury bonds, bills)     │           │ (Banknotes and coins)       │ │
    │   └─────────────────────────────┘           └─────────────────────────────┘ │
    │                                             │                               │
    │   ┌─────────────────────────────┐           ┌─────────────────────────────┐ │
    │   │ Foreign Exchange Reserves   │           │ Bank Reserves               │ │
    │   │ (Foreign currencies, gold)  │           │ (Deposits of commercial     │ │
    │   └─────────────────────────────┘           │  banks at central bank)     │ │
    │                                             └─────────────────────────────┘ │
    │   ┌─────────────────────────────┐           ┌─────────────────────────────┐ │
    │   │ Loans to Banks              │           │ Government Deposits         │ │
    │   │ (Discount window, repos)    │           │ (Treasury account)          │ │
    │   └─────────────────────────────┘           └─────────────────────────────┘ │
    │                                             │                               │
    │   ┌─────────────────────────────┐           ┌─────────────────────────────┐ │
    │   │ Other Assets                │           │ Other Liabilities           │ │
    │   │ (Emergency lending,         │           │ (Capital accounts, IMF)     │ │
    │   │  crisis facilities)         │           └─────────────────────────────┘ │
    │   └─────────────────────────────┘                                           │
    │                                                                             │
    │   ───────────────────────────               ───────────────────────────     │
    │   TOTAL ASSETS                 =            TOTAL LIABILITIES               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Balance Sheet Expansion and Contraction

Central bank balance sheet size changes with policy actions. Expansion adds assets and liabilities. Contraction reduces them.

```
BALANCE SHEET EXPANSION (QE EXAMPLE)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BEFORE QE:                                                                │
    │   Assets: $4 trillion          Liabilities: $4 trillion                     │
    │   ├── Securities: $3T          ├── Currency: $2T                            │
    │   └── Other: $1T               └── Reserves: $2T                            │
    │                                                                             │
    │                                                                             │
    │   QE OPERATION: Central bank buys $2 trillion in bonds                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK ──────$2 trillion──────────────────► COMMERCIAL BANKS │   │
    │   │                     (payment for bonds)                             │   │
    │   │                                                                     │   │
    │   │  CENTRAL BANK ◄─────$2 trillion bonds───────────── COMMERCIAL BANKS │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   AFTER QE:                                                                 │
    │   Assets: $6 trillion          Liabilities: $6 trillion                     │
    │   ├── Securities: $5T (+$2T)   ├── Currency: $2T (unchanged)                │
    │   └── Other: $1T               └── Reserves: $4T (+$2T)                     │
    │                                                                             │
    │   Key insight: QE expands both sides of the balance sheet equally.          │
    │   Reserves increase by the amount of asset purchases.                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Currency Issuance

### Sole Right to Issue Currency

Central banks have the exclusive legal authority to issue banknotes and coins. This monopoly ensures uniformity and public confidence in the currency.

How it works: The central bank prints notes and mints coins. These are distributed to commercial banks in exchange for reserves. The public obtains currency by withdrawing from bank accounts. The central bank's liability (currency) is matched by assets (securities, foreign reserves) that back the currency.

```
CURRENCY ISSUANCE PROCESS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STEP 1: Central bank prints banknotes or mints coins                      │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 2: Commercial bank requests currency                                 │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 3: Central bank debits bank's reserve account                        │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 4: Central bank ships physical currency to commercial bank           │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 5: Commercial bank holds currency in vault or ATMs                   │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 6: Customer withdraws cash from bank account                         │
    │        │                                                                    │
    │        ▼                                                                    │
    │   STEP 7: Currency enters circulation                                       │
    │                                                                             │
    │                                                                             │
    │   ACCOUNTING ENTRIES:                                                       │
    │                                                                             │
    │   Central Bank:                                                             │
    │   ├── Debit: Bank Reserves (liability decreases)                            │
    │   └── Credit: Currency in Circulation (liability increases)                 │
    │                                                                             │
    │   Commercial Bank:                                                          │
    │   ├── Debit: Vault Cash (asset increases)                                   │
    │   └── Credit: Reserve Account at Central Bank (asset decreases)             │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Banker to Banks

### Reserve Accounts

Commercial banks maintain reserve accounts at the central bank. These accounts are used for interbank settlement and to meet reserve requirements.

How it works: Each commercial bank has a digital account at the central bank. When Bank A pays Bank B, the central bank debits Bank A's account and credits Bank B's account. These transfers are final and irrevocable. The accounts earn interest (IORB rate) in most jurisdictions.

```
RESERVE ACCOUNT STRUCTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CENTRAL BANK LEDGER                                                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Account Holder              │ Balance ($ millions)                 │   │
    │   │  ────────────────────────────│──────────────────────────────────────│   │
    │   │  Bank of America             │ 150,000                              │   │
    │   │  JPMorgan Chase              │ 200,000                              │   │
    │   │  Wells Fargo                 │ 120,000                              │   │
    │   │  Citibank                    │ 90,000                               │   │
    │   │  Goldman Sachs               │ 40,000                               │   │
    │   │  Morgan Stanley              │ 35,000                               │   │
    │   │  Other Banks                 │ 250,000                              │   │
    │   │  ────────────────────────────│──────────────────────────────────────│   │
    │   │  Total Bank Reserves         │ 885,000                              │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   These accounts are:                                                       │
    │   ├── Digital only (no physical cash)                                       │
    │   ├── Interest-bearing (IORB rate)                                          │
    │   ├── Used for real-time interbank settlement                               │
    │   ├── No credit risk (central bank liability)                               │
    │   └── Only accessible to commercial banks                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Payment System Operation

Central banks operate or oversee real-time gross settlement (RTGS) systems that process large-value interbank payments.

How it works: The RTGS system settles each payment individually, in real time, using central bank reserves. Once settled, the payment is final and irrevocable. This eliminates credit risk between banks. Major RTGS systems include Fedwire (US), TARGET2 (Eurozone), CHAPS (UK), and BOJ-NET (Japan).

```
RTGS SETTLEMENT MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────┐                                      ┌─────────────┐      │
    │   │   Bank A    │                                      │   Bank B    │      │
    │   │             │                                      │             │      │
    │   │ Reserves:   │                                      │ Reserves:   │      │
    │   │ $100M       │                                      │ $50M        │      │
    │   └──────┬──────┘                                      └──────┬──────┘      │
    │          │                                                    │             │
    │          │  Bank A instructs RTGS to pay $10M to Bank B       │             │
    │          │                                                    │             │
    │          ▼                                                    ▼             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                       CENTRAL BANK RTGS SYSTEM                      │   │
    │   │                                                                     │   │
    │   │   1. Verify Bank A has sufficient reserves ($100M ≥ $10M)           │   │
    │   │   2. Debit Bank A reserve account: $100M → $90M                     │   │
    │   │   3. Credit Bank B reserve account: $50M → $60M                     │   │
    │   │   4. Send confirmation to both banks                                │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Result: Payment is final and irrevocable. No credit risk.                 │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Banker to Government

### Government Account

The central bank maintains the government's main checking account. Tax receipts flow into this account. Government payments flow out.

How it works: When taxpayers pay taxes, funds move from commercial bank accounts to the government's account at the central bank. When the government pays salaries or suppliers, funds move from the central bank account to commercial bank accounts. This is how fiscal policy interacts with the monetary system.

```
GOVERNMENT ACCOUNT OPERATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TAX COLLECTION:                                                           │
    │                                                                             │
    │   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐                   │
    │   │ Taxpayer    │────►│Commercial   │────►│ Central     │                   │
    │   │             │     │ Bank        │     │ Bank        │                   │
    │   │             │     │             │     │ (Govt Acct) │                   │
    │   └─────────────┘     └─────────────┘     └─────────────┘                   │
    │                                                                             │
    │   Effect: Private bank reserves decrease. Government balance increases.     │
    │                                                                             │
    │                                                                             │
    │   GOVERNMENT SPENDING:                                                      │
    │                                                                             │
    │   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐                   │
    │   │ Central     │────►│Commercial   │────►│ Supplier    │                   │
    │   │ Bank        │     │ Bank        │     │             │                   │
    │   │ (Govt Acct) │     │             │     │             │                   │
    │   └─────────────┘     └─────────────┘     └─────────────┘                   │
    │                                                                             │
    │   Effect: Private bank reserves increase. Government balance decreases.     │
    │                                                                             │
    │                                                                             │
    │   DEBT MANAGEMENT:                                                          │
    │                                                                             │
    │   The central bank may act as fiscal agent for government debt issuance.    │
    │   It coordinates Treasury auctions, processes interest payments, and        │
    │   manages maturing securities.                                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Lender of Last Resort

### Bagehot's Principle

The lender of last resort function is the central bank's responsibility to provide emergency liquidity to solvent but illiquid banks during crises. Walter Bagehot articulated the principle in 1873.

How it works: When a bank faces a sudden withdrawal of deposits (bank run), it may not have enough liquid assets to meet demand even though its long-term assets exceed liabilities. The central bank lends cash to the bank against good collateral at a penalty rate. This stops the run and prevents contagion.

```
LENDER OF LAST RESORT FRAMEWORK

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BAGEHOT'S PRINCIPLES (1873):                                              │
    │                                                                             │
    │   1. Lend freely                                                            │
    │   2. At a penalty rate                                                      │
    │   3. Against good collateral                                                │
    │   4. To solvent but illiquid institutions                                   │
    │                                                                             │
    │                                                                             │
    │   DISCOUNT WINDOW OPERATION:                                                │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   DISTRESSED BANK ──► Central Bank ──► LIQUIDITY PROVIDED           │   │
    │   │        │                    │                    │                  │   │
    │   │        ▼                    ▼                    ▼                  │   │
    │   │   Solvent but           Good              Penalty Rate              │   │
    │   │   Illiquid?            Collateral?        (Policy + Spread)         │   │
    │   │        │                    │                    │                  │   │
    │   │        └────────────┬───────┘                    │                  │   │
    │   │                     ▼                            ▼                  │   │
    │   │                YES + YES ──────────────────► APPROVED               │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   TIERS OF DISCOUNT WINDOW (Federal Reserve):                               │
    │                                                                             │
    │   Primary Credit:                                                           │
    │   ├── For financially sound institutions                                    │
    │   ├── Rate = Policy Rate + 0.50%                                            │
    │   └── No questions asked for first 90 days                                  │
    │                                                                             │
    │   Secondary Credit:                                                         │
    │   ├── For institutions not qualifying for primary                           │
    │   ├── Rate = Policy Rate + 1.00%                                            │
    │   └── Greater restrictions                                                  │
    │                                                                             │
    │   Seasonal Credit:                                                          │
    │   ├── For small institutions with seasonal patterns                         │
    │   ├── Rate = average of market rates                                        │
    │   └── Up to 9 months                                                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Preventing Contagion

The lender of last resort function prevents bank runs from spreading across the financial system. The mere existence of the facility often prevents runs from starting.

How it works: Depositors know that the central bank will provide liquidity to solvent banks. This reduces their incentive to withdraw. If a run does occur, the central bank's lending stops it. The discount window was used extensively during the 2008 financial crisis and the 2023 regional banking stress (Silicon Valley Bank, Signature Bank, First Republic).

## Financial Stability

### Macroprudential Regulation

Central banks are responsible for monitoring and mitigating systemic risk in the financial system. This is called macroprudential regulation.

How it works: Unlike microprudential regulation (supervising individual banks), macroprudential regulation looks at the system as a whole. Tools include countercyclical capital buffers (increase capital requirements during booms), stress tests (simulate crisis scenarios), and loan-to-value ratio limits for mortgages.

```
MACROPRUDENTIAL TOOLS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   TOOL                      │ PURPOSE                     │ TIMING          │
    │   ──────────────────────────│─────────────────────────────│───────────────  │
    │   Countercyclical Capital   │ Build capital buffers       │ Increase in     │
    │   Buffer (CCyB)             │ during booms for use in     │ booms,          │
    │                             │ busts                       │ release in      │
    │                             │                             │ busts           │
    │   ──────────────────────────│─────────────────────────────│───────────────  │
    │   Stress Tests              │ Identify vulnerabilities    │ Annual          │
    │                             │ under adverse scenarios     │                 │
    │   ──────────────────────────│─────────────────────────────│───────────────  │
    │   Loan-to-Value (LTV)       │ Limit mortgage borrowing    │ As needed       │
    │   Limits                    │ to prevent housing bubble   │                 │
    │   ──────────────────────────│─────────────────────────────│───────────────  │
    │   Debt-to-Income (DTI)      │ Limit household leverage    │ As needed       │
    │   Limits                    │                             │                 │
    │   ──────────────────────────│─────────────────────────────│───────────────  │
    │   Sectoral Capital          │ Target specific sectors     │ As needed       │
    │   Requirements              │ (commercial real estate,    │                 │
    │                             │  consumer lending)          │                 │
    │   ──────────────────────────│─────────────────────────────│───────────────  │
    │   Liquidity Coverage Ratio  │ Ensure sufficient high-     │ Continuous      │
    │   (LCR)                     │ quality liquid assets       │                 │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Central Bank Independence

### Why Independence Matters

Central bank independence is the freedom of the central bank from political influence in conducting monetary policy. Independent central banks achieve lower inflation without sacrificing growth.

How it works: Politicians face pressure to create unexpected inflation before elections to temporarily boost output. Markets anticipate this, resulting in higher inflation without output gains. An independent central bank resists this pressure, maintaining credibility and low inflation.

```
INDEPENDENCE DIMENSIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DIMENSION              │ MEANING                       │ COMMON PRACTICE  │
    │   ───────────────────────│───────────────────────────────│───────────────── │
    │   Instrument             │ Central bank can choose       │ Universal        │
    │   Independence           │ policy tools freely           │                  │
    │   ───────────────────────│───────────────────────────────│───────────────── │
    │   Goal Independence      │ Central bank sets policy      │ Less common      │
    │                          │ objectives                    │ (government      │
    │                          │                               │ typically sets   │
    │                          │                               │ mandate)         │
    │   ───────────────────────│───────────────────────────────│───────────────── │
    │   Personnel              │ Governors have fixed terms,   │ Common           │
    │   Independence           │ cannot be fired for policy    │                  │
    │                          │ disagreements                 │                  │
    │   ───────────────────────│───────────────────────────────│───────────────── │
    │   Financial              │ Central bank controls own     │ Common           │
    │   Independence           │ budget                        │                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Central Bank Credibility

Credibility is the public's belief that the central bank will achieve its stated objectives. Credible central banks achieve policy goals more easily.

How it works: If a central bank is credible, its inflation target anchors expectations. Workers and businesses set wages and prices assuming inflation will hit the target. This makes actual inflation easier to control. If credibility is lost, breaking high inflation expectations requires painful recessions (Volcker disinflation 1979-1982).

## International Role

### Foreign Exchange Reserves

Central banks hold foreign currency reserves to intervene in currency markets and maintain confidence in the domestic currency.

How it works: The central bank accumulates foreign currencies (primarily US dollars, euros) by purchasing them in exchange for domestic currency. These reserves can be sold to support the domestic currency during depreciation pressure. Reserves also serve as a buffer against external shocks.

```
FOREIGN RESERVE COMPOSITION (Global)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Total Global Reserves: ~$12 trillion                                     │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Currency              │ Share (%)                                   │   │
    │   │  ──────────────────────│─────────────────────────────────────────────│   │
    │   │  US Dollar             │ 58%                                         │   │
    │   │  Euro                  │ 20%                                         │   │
    │   │  Japanese Yen          │ 5%                                          │   │
    │   │  British Pound         │ 5%                                          │   │
    │   │  Chinese Renminbi      │ 3%                                          │   │
    │   │  Canadian Dollar       │ 2%                                          │   │
    │   │  Australian Dollar     │ 2%                                          │   │
    │   │  Other                 │ 5%                                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   Gold also held as reserve (about 10% of total reserve value).           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Currency Swaps

Central banks establish bilateral currency swap lines to provide foreign currency liquidity during crises.

How it works: Two central banks agree to exchange currencies up to a specified limit. A central bank facing dollar shortage can borrow dollars from the Federal Reserve, using its own currency as collateral. This provides liquidity without depleting foreign reserves.

```
FEDERAL RESERVE STANDING SWAP LINES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Federal Reserve (USD) ──Swap Line──► Bank of Canada (CAD)               │
    │                     │                                                      │
    │                     ├──Swap Line──► Bank of England (GBP)                  │
    │                     │                                                      │
    │                     ├──Swap Line──► European Central Bank (EUR)            │
    │                     │                                                      │
    │                     ├──Swap Line──► Bank of Japan (JPY)                    │
    │                     │                                                      │
    │                     └──Swap Line──► Swiss National Bank (CHF)              │
    │                                                                             │
    │   These are standing, unlimited swap lines established in 2013.           │
    │   Used extensively during 2008 crisis and COVID-19 pandemic.              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Major Central Banks

```
MAJOR CENTRAL BANKS COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Central Bank         │ Currency │ Policy Rate │ RTGS System │ CBDC Status│
    │   ─────────────────────│──────────│─────────────│─────────────│────────────│
    │   Federal Reserve      │ USD      │ 5.25-5.50%  │ Fedwire     │ Research   │
    │   (USA)                │          │ (as of 2024)│             │            │
    │   ─────────────────────│──────────│─────────────│─────────────│────────────│
    │   European Central     │ EUR      │ 4.50%       │ TARGET2     │ Digital    │
    │   Bank (Eurozone)      │          │             │             │ Euro       │
    │   ─────────────────────│──────────│─────────────│─────────────│────────────│
    │   Bank of England      │ GBP      │ 5.25%       │ CHAPS       │ Digital    │
    │   (UK)                 │          │             │             │ Pound      │
    │   ─────────────────────│──────────│─────────────│─────────────│────────────│
    │   Bank of Japan (JP)   │ JPY      │ -0.10%      │ BOJ-NET     │ Digital    │
    │                        │          │             │             │ Yen        │
    │   ─────────────────────│──────────│─────────────│─────────────│────────────│
    │   People's Bank of     │ CNY      │ 3.45%       │ CNAPS       │ e-CNY      │
    │   China (CN)           │          │             │             │ (live)     │
    │   ─────────────────────│──────────│─────────────│─────────────│────────────│
    │   Swiss National Bank  │ CHF      │ 1.75%       │ SIC5        │ Project    │
    │   (CH)                 │          │             │             │ Helvetia   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
CENTRAL BANK FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Monetary Base (M0) = Currency in Circulation + Bank Reserves            │
    │                                                                             │
    │   Required Reserves = Reserve Requirement Ratio × Deposits                 │
    │                                                                             │
    │   Excess Reserves = Total Reserves - Required Reserves                    │
    │                                                                             │
    │   Money Multiplier (simple) = 1 / Reserve Requirement Ratio                │
    │                                                                             │
    │   Policy Rate Corridor = Lending Rate - Deposit Rate                       │
    │                                                                             │
    │   Taylor Rule: i = r* + π + 0.5(π - π*) + 0.5(y - y*)                     │
    │                                                                             │
    │   Real Interest Rate = Nominal Rate - Inflation Rate                       │
    │                                                                             │
    │   Central Bank Balance Sheet Identity: Assets = Liabilities                │
    │                                                                             │
    │   Seigniorage = Face Value of Currency - Production Cost                   │
    │                                                                             │
    │   Discount Window Penalty (Primary) = Policy Rate + 0.50%                  │
    │                                                                             │
    │   Discount Window Penalty (Secondary) = Policy Rate + 1.00%                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Central bank is apex financial institution managing currency, money supply, and interest rates.

2. Core functions: monetary policy, currency issuance, banker to banks, banker to government, lender of last resort, payment systems oversight, financial stability.

3. Mandates vary: Fed (dual mandate: price stability + employment), ECB (price stability hierarchical), others.

4. Monetary policy tools: policy rate, open market operations, reserve requirements, discount window, QE, negative rates, forward guidance, YCC.

5. Policy rate transmission: rate changes flow through interbank rates to lending/deposit rates to spending to inflation/output.

6. Balance sheet: assets (securities, foreign reserves, loans) = liabilities (currency, reserves, government deposits).

7. QE expands balance sheet: buys assets, creates reserves. Balance sheet grows.

8. Currency issuance: central bank has monopoly. Banks exchange reserves for physical currency.

9. Reserve accounts: commercial banks hold digital accounts at central bank for settlement.

10. RTGS systems: real-time gross settlement using central bank reserves. Final and irrevocable.

11. Government account: central bank holds Treasury's checking account. Tax and spending flows.

12. Lender of last resort: Bagehot's principle: lend freely at penalty rate against good collateral to solvent but illiquid banks.

13. Discount window tiers: primary (penalty +0.50%), secondary (+1.00%), seasonal.

14. Financial stability: macroprudential tools (CCyB, stress tests, LTV limits, LCR).

15. Central bank independence: instrument independence common. Reduces time-inconsistency problem.

16. Credibility: public belief that central bank will achieve targets. Makes policy more effective.

17. Foreign reserves: held in major currencies (USD 58%, EUR 20%). Provide currency intervention capability.

18. Currency swaps: bilateral arrangements for foreign currency liquidity during crises.

19. Major central banks: Fed, ECB, BOE, BOJ, PBOC, SNB have different policy rates and CBDC progress.

20. Central bank is the ultimate source of domestic currency and the settlement asset for all interbank payments.

*This documentation belongs to https://github.com/InterCentury*
