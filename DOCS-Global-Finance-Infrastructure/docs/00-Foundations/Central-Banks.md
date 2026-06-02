# 01 - Central Banks

## Documentation Overview

Central banks are the cornerstone of global financial infrastructure. They issue currency, manage monetary policy, oversee payment systems, act as lenders of last resort, and maintain financial stability. This document covers the core functions, operational tools, and infrastructure roles of major central banks including the Federal Reserve (US), European Central Bank (ECB), Bank of England (BoE), Bank of Japan (BOJ), and People's Bank of China (PBOC).

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the core functions of central banks                            │
    │   Learn monetary policy implementation tools                                │
    │   Study central bank payment and settlement systems                         │
    │   Analyze lender of last resort operations                                  │
    │   Examine reserve management and foreign exchange                           │
    │   Understand central bank digital currency (CBDC) frameworks                │
    │   Provide reference for financial system developers                         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Theory of Operation

### Central Bank Functions Overview

```
Function Type          │ Structural Mechanism                  │ Functional System Impact
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Monetary Policy        │ Interest rate setting, open market    │ Controls inflation; stabilizes economic cycles
                       │ operations, reserve requirements.     │
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Currency Issuance      │ Sole legal authority to print         │ Maintains public confidence in money;
                       │ banknotes and mint coins.             │ enables domestic payment system.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Payment System         │ Operation of RTGS (Fedwire, TARGET2,  │ Ensures final, irrevocable settlement in
Oversight              │ CHAPS); oversight of retail systems.  │ central bank money; reduces systemic risk.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Lender of Last Resort  │ Discount window lending against       │ Prevents bank runs; provides emergency
                       │ eligible collateral at penalty rate.  │ liquidity to solvent but illiquid institutions.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Foreign Exchange       │ Holding foreign currency reserves;    │ Stabilizes exchange rates; supports
Reserve Management     │ market intervention when needed.      │ international trade and financial stability.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

### Monetary Policy Transmission Mechanism

```
Central Bank Action    │ Market Response                        │ Economic Impact
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Raise policy rate      │ Higher interbank lending rates;       │ Reduced borrowing; lower spending;
                       │ increased bond yields.                │ inflation decreases.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Sell government bonds  │ Lower bond prices; higher yields;     │ Tighter liquidity; reduced money supply;
(Open market sale)     │ banks have less reserve liquidity.    │ slower economic growth.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Lower reserve          │ Banks have more lendable funds;       │ Increased loan origination; higher
requirement            │ interbank rates decline.              │ money supply; stimulates activity.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Quantitative easing    │ Central bank buys assets; injects     │ Lower long-term interest rates;
(QE asset purchase)    │ liquidity; bank reserves increase.    │ asset prices rise; economy stimulated.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Currency intervention  │ Central bank buys/sells foreign FX;   │ Exchange rate moves toward target;
(Buy local currency)   │ domestic money supply contracts.      │ import prices affected.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Forward guidance       │ Market expectations shift; yield      │ Long-term rates adjust without
(promise future path)  │ curve reprices based on guidance.     │ immediate policy action.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

## Major Central Banks Overview

### Central Bank Comparison

```
Central Bank           │ Currency │ Policy Rate   │ RTGS System │ CBDC Status
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
Federal Reserve (USA)  │ USD      │ 5.25-5.50%    │ Fedwire     │ In research (Project Cedar)
                       │          │ (as of 2024)  │             │
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
European Central Bank  │ EUR      │ 4.50%         │ TARGET2     │ Digital Euro (in progress)
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
Bank of England (UK)   │ GBP      │ 5.25%         │ CHAPS       │ Digital Pound (in progress)
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
Bank of Japan          │ JPY      │ -0.10%        │ BOJ-NET     │ Digital Yen (in progress)
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
People's Bank of China │ CNY      │ 3.45%         │ CNAPS       │ e-CNY (live pilot, 260M users)
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
Swiss National Bank    │ CHF      │ 1.75%         │ SIC5        │ Project Helvetia (wholesale pilot)
───────────────────────│──────────│───────────────│─────────────│─────────────────────────────────────────────────────
```

## Payment Systems Operated by Central Banks

### Real-Time Gross Settlement (RTGS) Systems

```
RTGS System    │ Operator         │ Daily Volume    │ Settlement   │ Operating Hours
               │                  │ (USD equivalent)│ Asset        │
───────────────│──────────────────│─────────────────│──────────────│────────────────────────────────────────────────────
Fedwire        │ Federal Reserve  │ ~$2.5 trillion  │ Central bank │ 22 hours (US time)
               │                  │                 │ reserves     │
───────────────│──────────────────│─────────────────│──────────────│────────────────────────────────────────────────────
TARGET2        │ ECB/Eurosystem   │ ~$2.0 trillion  │ Central bank │ 24/7 for some operations
               │                  │                 │ reserves     │
───────────────│──────────────────│─────────────────│──────────────│────────────────────────────────────────────────────
CHAPS          │ Bank of England  │ ~$500 billion   │ Central bank │ 6:00-18:00 (UK time)
               │                  │                 │ reserves     │
───────────────│──────────────────│─────────────────│──────────────│────────────────────────────────────────────────────
BOJ-NET        │ Bank of Japan    │ ~$400 billion   │ Central bank │ 9:00-17:00 (JST)
               │                  │                 │ reserves     │
───────────────│──────────────────│─────────────────│──────────────│────────────────────────────────────────────────────
CNAPS          │ People's Bank    │ ~$5 trillion    │ Central bank │ 8:30-17:00 (CST)
               │ of China         │                 │ reserves     │
───────────────│──────────────────│─────────────────│──────────────│────────────────────────────────────────────────────
```

### RTGS Key Features

```
Feature                    │ Structural Mechanism                  │ Functional System Impact
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Individual settlement      │ Each payment processed and settled    │ No netting; eliminates counterparty credit
                           │ separately, not batched.              │ risk between participants.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Settlement finality        │ Once settled, transaction is          │ Irrevocable transfer; reduces legal
                           │ irrevocable and legally binding.      │ uncertainty and systemic risk.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Central bank money         │ Settlement occurs in central bank     │ Risk-free settlement asset; no credit
                           │ reserve accounts.                     │ risk on the settlement medium itself.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Intraday liquidity         │ Central bank provides interest-free   │ Enables continuous settlement without
                           │ intraday credit against collateral.   │ requiring end-of-day positive balances.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Liquidity saving mechanism │ Queuing, offsetting, and priority     │ Reduces liquidity needs while maintaining
(LSM)                      │ processing of payments.               │ RTGS risk reduction benefits.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

## Monetary Policy Implementation

### Monetary Policy Toolkit

```
Policy Tool                │ Structural Mechanism                  │ Functional System Impact
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Policy rate                │ Interest rate on reserve balances;    │ Primary price stability tool; influences
(Fed Funds, Main Refi,     │ overnight reverse repurchase          │ all other interest rates in economy.
Bank Rate)                 │ agreements (ON RRP).                  │
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Open market operations     │ Central bank buys or sells            │ Adjusts reserve levels daily; implements
(OMO)                      │ government securities in open market. │ policy rate target.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Reserve requirements       │ Mandated minimum reserves as          │ Less common today (zero in UK, Canada,
                           │ percentage of transaction deposits.   │ Australia); historically controlled lending.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Standing facilities        │ Deposit facility (floor) and lending  │ Creates interest rate corridor; provides
                           │ facility (ceiling) at policy rate ±   │ liquidity and deposit services daily.
                           │ spread.                               │
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Quantitative easing (QE)   │ Large-scale purchases of government   │ Lowers long-term rates; injects liquidity
                           │ bonds, MBS, or corporate debt.        │ during zero-lower-bound periods.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Forward guidance           │ Public communication of expected      │ Shapes market expectations; reduces
                           │ future policy path.                   │ uncertainty; extends policy influence.
───────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

### Interest Rate Corridor System

```
Corridor Component        │ Structural Mechanism                  │ Functional System Impact
──────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Deposit facility (floor)  │ Banks can park excess reserves        │ Sets minimum rate for overnight money;
                          │ overnight at central bank at policy   │ prevents rates falling below floor.
                          │ rate minus spread.                    │
──────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Policy rate (target)      │ Announced target for overnight        │ Guides interbank lending rates toward
                          │ interbank lending rate.               │ desired level.
──────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Lending facility (ceiling)│ Banks can borrow overnight against    │ Sets maximum rate for overnight money;
                          │ eligible collateral at policy rate    │ prevents rates rising above ceiling.
                          │ plus spread.                          │
──────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Corridor width            │ Difference between lending and        │ Controls volatility; typical width
                          │ deposit rates (50-100 basis points).  │ 50-100 bps.
──────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

## Lender of Last Resort (LOLR) Function

### Discount Window Framework

```
LOLR Component           │ Structural Mechanism                  │ Functional System Impact
─────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Bagehot's Principle      │ "Lend freely at a penalty rate        │ Prevents bank runs without encouraging
(1873)                   │ against good collateral."             │ moral hazard; supports solvent banks.
─────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Eligibility criteria     │ Solvent but illiquid institutions;    │ Filters out insolvent banks; limits
                         │ good collateral required; penalty     │ central bank credit risk exposure.
                         │ rate above market.                    │
─────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Primary credit           │ For financially sound institutions;   │ Main discount window facility; no
(Federal Reserve)        │ rate = policy rate + 0.50%;           │ questions asked for first 90 days.
                         │ overnight to 90-day terms.            │
─────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Secondary credit         │ For institutions not qualifying for   │ Higher penalty (policy rate + 1.00%);
                         │ primary; greater restrictions.        │ subject to enhanced oversight.
─────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Seasonal credit          │ For smaller institutions with         │ Supports agricultural and tourist banks;
                         │ seasonal liquidity patterns; rate     │ up to 9 months term.
                         │ = average of selected market rates.   │
─────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

## Reserve Management and Balance Sheet

### Central Bank Balance Sheet Structure

```
Balance Sheet Side      │ Component                             │ Functional System Impact
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
ASSETS                  │ Government securities (Treasury       │ Primary asset; earns interest; created
                        │ bonds, bills)                         │ through open market purchases.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
ASSETS                  │ Foreign exchange reserves (foreign    │ Supports currency intervention; backs
                        │ currencies, gold, SDR)                │ domestic money supply.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
ASSETS                  │ Loans to banks (discount window,      │ Emergency liquidity; lender of last
                        │ repo agreements)                      │ resort function.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
LIABILITIES             │ Currency in circulation (banknotes    │ Non-interest bearing; primary liability;
                        │ and coins)                            │ represents public's cash holdings.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
LIABILITIES             │ Reserve balances (bank deposits at    │ Interest-bearing; settlement asset for
                        │ central bank)                         │ interbank payments.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
LIABILITIES             │ Government deposits (Treasury         │ Fiscal agent function; government
                        │ accounts)                             │ spending and tax collection.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
IDENTITY                │ TOTAL ASSETS = TOTAL LIABILITIES      │ Balance sheet always balances by
                        │                                       │ accounting construction.
────────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

### Reserve Requirement Formulas

```
Formula Concept        │ Mathematical Expression                │ Functional System Impact
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Required reserves      │ R_req = RR_ratio × D_trans            │ Minimum reserves bank must hold
                       │                                       │ against transaction deposits.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Excess reserves        │ R_excess = R_actual - R_req           │ Lendable funds beyond regulatory
                       │                                       │ minimum.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Money multiplier       │ m = 1 / RR_ratio                      │ Maximum potential money creation
(simple model)         │                                       │ from initial deposit.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Total money creation   │ ΔM = Initial_deposit × m              │ Expansion of money supply through
                       │                                       │ fractional reserve banking.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
EXAMPLE (RR = 10%)     │ R_req = 0.10 × $100M = $10M           │ Bank must hold $10M in reserves
                       │ m = 1 / 0.10 = 10                     │ against $100M deposits.
                       │ ΔM = $1M × 10 = $10M                  │ $1M deposit can become $10M supply.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
NOTE                   │ Many central banks (Canada, UK,       │ Zero reserve requirements; interest
                       │ Australia) have zero RR.              │ on reserves is primary policy tool.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

### Typical Federal Reserve Balance Sheet (simplified)

```
Asset Component        │ Approximate Value                     │ Liability Component    │ Approximate Value
───────────────────────│───────────────────────────────────────│────────────────────────│─────────────────────────────────────────
US Treasury securities │ ~$5 trillion                          │ Currency in circulation│ ~$2.3 trillion
───────────────────────│───────────────────────────────────────│────────────────────────│─────────────────────────────────────────
Mortgage-backed        │ ~$2.5 trillion                        │ Reserve balances       │ ~$3.5 trillion
securities (MBS)       │                                       │                        │
───────────────────────│───────────────────────────────────────│────────────────────────│─────────────────────────────────────────
Other assets           │ ~$0.5 trillion                        │ Reverse repo balances  │ ~$1.5 trillion
(emergency lending,    │                                       │                        │
crisis facilities)     │                                       │                        │
───────────────────────│───────────────────────────────────────│────────────────────────│─────────────────────────────────────────
TOTAL ASSETS           │ ~$8 trillion                          │ TOTAL LIABILITIES      │ ~$8 trillion
───────────────────────│───────────────────────────────────────│────────────────────────│─────────────────────────────────────────
```

## Central Bank Digital Currency (CBDC)

### CBDC Architecture Types

```
Architecture Type      │ Structural Mechanism                  │ Functional System Impact
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Direct CBDC (Retail)   │ Central bank holds all retail         │ No commercial bank intermediation; central
                       │ accounts; processes all payments      │ bank directly services public.
                       │ directly. Example: No intermediaries. │
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Indirect CBDC          │ Central bank issues wholesale CBDC    │ Commercial banks distribute to public;
(Two-tier)             │ to commercial banks; banks            │ preserves existing banking model.
                       │ distribute to public.                 │
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Hybrid CBDC            │ Central bank handles wholesale and    │ Central bank can see all transactions
                       │ settlement; private intermediaries   │ (privacy concerns); balances control
                       │ handle customer-facing services.      │ and oversight.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

### CBDC Design Dimensions

```
Design Dimension       │ Options Available                      │ Functional System Impact
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Access                 │ Account-based vs Token-based          │ Account: identity-linked, regulated.
                       │                                       │ Token: bearer instrument, more anonymous.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Intermediation         │ Direct vs Indirect vs Hybrid          │ Determines role of commercial banks in
                       │                                       │ CBDC distribution.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Remuneration           │ Interest-bearing vs Zero interest     │ Interest-bearing competes with bank deposits;
                       │                                       │ zero interest limits disintermediation.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Anonymity              │ Anonymous vs Identified vs Tiered     │ Trade-off between privacy and anti-money
                       │                                       │ laundering (AML) compliance.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Limits                 │ None vs Transaction caps vs           │ Controls CBDC usage; prevents bank runs
                       │ Balance caps                          │ by limiting convertibility from deposits.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Technology             │ DLT vs Traditional centralized        │ DLT enables programmability and atomic
                       │ ledger                                │ settlement; centralized is simpler.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
Cross-border           │ Compatible vs Proprietary             │ Compatible enables international
                       │                                       │ interoperability; proprietary isolates.
───────────────────────│───────────────────────────────────────│───────────────────────────────────────────────────────
```

### Global CBDC Status (2024-2025)

```
Status Level          │ Countries / Projects                   │ Functional System Impact
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
LIVE (Full launch)    │ Bahamas (Sand Dollar), Nigeria         │ Operational retail CBDC; public can
                      │ (eNaira), Jamaica (JAM-DEX),           │ transact in digital central bank money.
                      │ Eastern Caribbean (DCash)              │
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
PILOT (Large scale)   │ China (e-CNY - 260M users),            │ Large-scale testing; real transactions
                      │ India (e-Rupee), Brazil (Drex),        │ with limited user base.
                      │ Russia (Digital Ruble)                 │
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
PILOT (Wholesale)     │ Switzerland (Project Helvetia),        │ Wholesale CBDC for interbank settlement;
                      │ Singapore (Project Ubin), France       │ not available to public.
                      │ (wCBDC experiments)                    │
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
IN PROGRESS           │ Eurozone (Digital Euro), UK            │ Research and development phase;
                      │ (Digital Pound), USA (Project Cedar),  │ policy decisions pending.
                      │ Japan, South Korea                     │
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
RESEARCH              │ Canada, Australia, Sweden (e-krona),   │ Early investigation; no launch commitment.
                      │ Israel, Norway                         │
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
NO PLANS / PAUSED     │ Germany (prefers digital euro),        │ No active CBDC program; may use other
                      │ Ecuador (ended), Finland (no need),    │ regional or global solutions.
                      │ Senegal (ended)                        │
──────────────────────│────────────────────────────────────────│────────────────────────────────────────────────────────
```

## Cross-Border Central Bank Cooperation

### Bilateral and Multilateral Arrangements

```
Cooperation Type     │ Structural Mechanism                  │ Functional System Impact
─────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Currency swap lines  │ Two central banks agree to exchange   │ Provides foreign currency liquidity during
                     │ currencies up to a predetermined      │ stress; prevents funding market freezes.
                     │ limit.                                │
─────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Federal Reserve      │ Standing arrangements with Bank of    │ USD liquidity available to major central
standing swap lines  │ Canada, Bank of England, ECB, Bank    │ banks during global stress events.
                     │ of Japan, Swiss National Bank.        │
─────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
mBridge (BIS)        │ DLT-based wholesale CBDC platform;    │ Reduces correspondent banking costs;
                     │ Participants: China, Hong Kong,       │ enables direct cross-border settlement.
                     │ Thailand, UAE, Saudi Arabia.          │
─────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Project Agorá (BIS)  │ Tokenized commercial bank deposits    │ Improves cross-border payment speed,
                     │ + wholesale CBDC; 7 central banks     │ transparency, and reduces counterparty
                     │ including Fed NY, BoE, BoJ, Banque    │ risk.
                     │ de France, SNB, Bank of Korea,        │
                     │ Bank of Mexico.                       │
─────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Project Nexus (BIS)  │ Links domestic fast payment systems   │ Enables instant cross-border retail
                     │ (FPS); participants: Malaysia,        │ payments; users pay as easily as domestic.
                     │ Philippines, Singapore, Thailand,     │
                     │ India (2024).                         │
─────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
```

## Oversight and Standards

### International Frameworks

```
Oversight Body      │ Structural Mechanism                  │ Functional System Impact
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
CPMI (Committee on  │ Hosted by Bank for International      │ Sets global standards for payment and
Payments and Market │ Settlements (BIS); 28 member          │ settlement systems; monitors compliance.
Infrastructures)    │ central banks.                        │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
PFMI (Principles    │ 24 principles for financial market    │ Reduces systemic risk; ensures resilience;
for Financial       │ infrastructures (FMIs).               │ promotes legal clarity and transparency.
Market              │                                       │
Infrastructures)    │                                       │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
```

### PFMI Key Principles for Central Banks

```
Principle           │ Requirement                           │ Functional System Impact
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 1:        │ FMI should have solid legal           │ Ensures settlement finality and netting
Legal basis         │ foundation in all relevant            │ enforceability across jurisdictions.
                    │ jurisdictions.                        │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 2:        │ Clear, transparent governance         │ Prevents conflicts of interest; ensures
Governance          │ arrangements with clear roles,        │ accountability and stakeholder representation.
                    │ responsibilities, and accountability. │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 3:        │ Comprehensive framework to manage     │ Identifies, monitors, and mitigates
Risk management     │ credit, liquidity, operational, and   │ all material risks to the FMI.
                    │ other risks.                          │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 4:        │ Measure and cover credit exposures    │ Prevents losses from participant default;
Credit risk         │ to participants.                      │ maintains financial integrity.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 5:        │ Require low-risk, highly liquid       │ Ensures collateral can be liquidated
Collateral          │ collateral with appropriate           │ quickly without price impact.
                    │ haircuts.                             │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 6:        │ Risk-based margin requirements for    │ Covers potential future exposure;
Margin              │ covered transactions.                 │ prevents under-collateralization.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 7:        │ Sufficient liquid resources to settle│ Enables timely settlement even under
Liquidity risk      │ obligations under extreme scenarios.  │ extreme market stress.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 8:        │ Final settlement occurs no later than│ Provides certainty to participants;
Settlement          │ end of value date; preferably real-   │ reduces legal and credit risk.
finality            │ time.                                 │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 9:        │ Use central bank money where          │ Eliminates credit risk on settlement
Money settlements   │ possible and practical.               │ asset.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Principle 10:       │ Clarify settlement finality for       │ Reduces legal uncertainty; ensures
Physical deliveries │ physically settled instruments.       │ delivery-versus-payment (DvP) integrity.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
```

## Operational Risk and Resilience

### Business Continuity and Cyber Security

```
Resilience Layer    │ Control Mechanism                     │ Functional System Impact
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Recovery Time       │ RTO < 2 hours for critical systems    │ Limits outage duration; maintains financial
Objective (RTO)     │                                       │ stability.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Recovery Point      │ RPO < 5 minutes data loss             │ Minimizes transaction loss during failover.
Objective (RPO)     │                                       │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Geographic          │ Minimum 2 data centers > 50 km apart  │ Survives regional disaster (natural, power,
redundancy          │                                       │ political).
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Annual testing      │ Full failover drills (minimum 2x per  │ Verifies recovery procedures work under
                    │ year)                                 │ realistic conditions.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Identity Management │ Multi-factor authentication for all  │ Prevents unauthorized access to critical
                    │ privileged access.                    │ systems.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Network Security    │ Air-gapped backup systems; TLS 1.3+   │ Protects against remote compromise;
                    │ encryption; multi-terabit DDoS        │ ensures communication confidentiality.
                    │ protection.                           │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Application         │ Regular penetration testing; bug      │ Identifies vulnerabilities before
Security            │ bounty programs; secure SDLC.         │ exploitation.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Data Protection     │ AES-256 encryption at rest; TLS       │ Protects sensitive financial data;
                    │ encryption in transit; hardware       │ HSMs protect cryptographic keys.
                    │ security modules (HSMs).              │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Monitoring          │ SIEM with real-time alerting; 24/7    │ Detects and responds to threats in
                    │ security operations center (SOC);     │ real time.
                    │ threat hunting.                       │
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Recovery            │ Offline air-gapped backups; manual    │ Survives ransomware; allows system
                    │ override capabilities; paper-based    │ restoration even if primary systems
                    │ fallback procedures.                  │ are compromised.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
```

## Central Bank Communications

### Forward Guidance Framework

```
Guidance Type       │ Structural Mechanism                  │ Functional System Impact
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Calendar-based      │ "Policy rate will remain at current   │ Provides certainty about time horizon;
                    │ level until Q2 2026."                 │ reduces market speculation.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
State-based         │ "Rates will not increase until        │ Conditions guidance on observable
(outcome)           │ inflation sustainably reaches 2%."    │ economic outcomes; more flexible.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
State-based         │ "Asset purchases will continue until  │ Clear numerical threshold; easy to
(threshold)         │ unemployment falls below 6.5%."       │ communicate and verify.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Open-ended          │ "Policy will remain accommodative for │ Maximum flexibility; least precise
                    │ an extended period."                  │ for market expectations.
────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
```

### Communication Channels

```
Channel                     │ Frequency                      │ Audience
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Monetary Policy Statement   │ 6-8 times per year             │ Public, financial markets
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Press Conference            │ After each policy meeting      │ Media, public
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Meeting Minutes             │ 3 weeks after policy meeting   │ Markets, analysts, academics
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Quarterly Monetary Policy   │ 4 times per year               │ Public, markets, media
Report                      │                                │
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Speeches by central bank    │ Ongoing (weekly/monthly)       │ Markets, experts, media
officials                   │                                │
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Economic Projections        │ 4 times per year               │ Markets, analysts
(dot plots)                 │                                │
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
Financial Stability Report  │ 1-2 times per year             │ Financial industry, public
────────────────────────────│────────────────────────────────│────────────────────────────────────────────────────────
```

## Formulas Quick Reference

```
Formula Concept        │ Mathematical Expression                │ Purpose
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Money multiplier       │ m = 1 / RR_ratio                      │ Maximum potential money creation
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Required reserves      │ R_req = RR_ratio × D_trans            │ Minimum reserves bank must hold
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Excess reserves        │ R_excess = R_actual - R_req           │ Lendable funds beyond requirements
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Policy rate corridor   │ Width = Lending_rate - Deposit_rate   │ Interest rate band width
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Real interest rate     │ r_real = r_nominal - π               │ Inflation-adjusted return
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Quantity theory        │ MV = PQ                               │ Money × Velocity = Price × Output
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Taylor rule            │ i = r* + π + 0.5(π - π*) +            │ Policy rate guidance formula
                       │     0.5(y - y*)                       │
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Reserve balance        │ R_balance = Assets - Currency -       │ Central bank liquidity calculation
                       │ Other_liabilities                     │
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Discount window        │ Rate_primary = Policy_rate + 0.50%    │ Cost of LOLR borrowing (primary)
penalty                │                                       │
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
Discount window        │ Rate_secondary = Policy_rate + 1.00%  │ Cost of LOLR borrowing (secondary)
penalty (secondary)    │                                       │
───────────────────────│───────────────────────────────────────│────────────────────────────────────────────────────────
```

## Summary

1. Core functions: Monetary policy, currency issuance, payment system oversight, lender of last resort, foreign reserve management.

2. Major central banks: Federal Reserve (USD), ECB (EUR), Bank of England (GBP), Bank of Japan (JPY), PBOC (CNY).

3. RTGS systems: Fedwire, TARGET2, CHAPS, BOJ-NET, CNAPS — settle large-value payments in central bank money.

4. Monetary policy tools: Policy rate, open market operations, reserve requirements, standing facilities, quantitative easing, forward guidance.

5. Interest rate corridor: Deposit facility (floor), lending facility (ceiling), policy rate (target).

6. Lender of last resort: Bagehot's principle — lend freely at penalty rate against good collateral to solvent but illiquid banks.

7. Balance sheet: Assets (government securities, FX reserves, loans) = Liabilities (currency, reserves, government deposits).

8. Reserve requirement: Formula R = RR × Deposits; money multiplier = 1 / RR (theoretical).

9. CBDC types: Direct (retail), indirect (two-tier), hybrid — with design dimensions (access, anonymity, limits, technology).

10. CBDC status: Live (Bahamas, Nigeria, Jamaica), pilot (China, India, Brazil), research (Eurozone, UK, USA).

11. Cross-border cooperation: Currency swap lines, mBridge, Project Agorá, Project Nexus.

12. Oversight standards: CPMI, PFMI (24 principles for financial market infrastructures).

13. Resilience requirements: RTO < 2 hours, RPO < 5 minutes, geographic redundancy, cyber controls (MFA, encryption, HSMs, offline backups).

14. Forward guidance: Calendar-based, state-based (outcome/threshold), open-ended — shapes market expectations.

15. Communications: Policy statements, press conferences, minutes, quarterly reports, speeches, dot plots (economic projections).

*This documentation belongs to https://github.com/InterCentury*