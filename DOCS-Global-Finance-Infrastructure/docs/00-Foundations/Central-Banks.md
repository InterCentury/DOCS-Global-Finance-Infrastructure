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
CENTRAL BANK CORE FUNCTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MONETARY POLICY                                                           │
    │   ├── Price stability (inflation targeting)                                 │
    │   ├── Interest rate setting (policy rate)                                   │
    │   ├── Open market operations (buy/sell securities)                          │
    │   ├── Reserve requirements                                                  │
    │   └── Quantitative easing (asset purchases)                                 │
    │                                                                             │
    │   CURRENCY ISSUANCE                                                         │
    │   ├── Sole right to issue banknotes and coins                               │
    │   ├── Maintain public confidence in currency                                │
    │   ├── Manage currency supply                                                │
    │   └── Combat counterfeiting                                                 │
    │                                                                             │
    │   PAYMENT SYSTEM OVERSIGHT                                                  │
    │   ├── Operate RTGS systems (Fedwire, TARGET2, CHAPS)                        │
    │   ├── Oversee retail payment systems                                        │
    │   ├── Ensure settlement finality                                            │
    │   └── Reduce systemic risk                                                  │
    │                                                                             │
    │   LENDER OF LAST RESORT                                                     │
    │   ├── Provide emergency liquidity to banks                                  │
    │   ├── Prevent bank runs                                                     │
    │   ├── Maintain financial stability                                          │
    │   └── Operate discount window                                               │
    │                                                                             │
    │   FOREIGN EXCHANGE RESERVE MANAGEMENT                                       │
    │   ├── Hold and manage foreign currency reserves                             │
    │   ├── Intervene in currency markets                                         │
    │   ├── Maintain exchange rate stability                                      │
    │   └── Support international trade                                           │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    MONETARY POLICY TRANSMISSION MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Central Bank Action              Market Response          Economic Impact│
    │   ──────────────────────────────────────────────────────────────────────── │
    │                                                                             │
    │   Raise policy rate         →    Higher bank rates    →    Reduced lending │
    │                                                                             │
    │   Sell government bonds     →    Lower bond prices    →    Higher yields   │
    │                             →    Tighter liquidity    →    Slower growth    │
    │                                                                             │
    │   Lower reserve requirement →    More lendable funds  →    Increased loans │
    │                                                                             │
    │   Quantitative easing       →    Buy assets           →    Inject liquidity│
    │                             →    Lower long-term rates→    Stimulate economy│
    │                                                                             │
    │   Currency intervention     →    Buy/sell foreign FX  →    Stabilize rate  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Major Central Banks Overview

### Central Bank Comparison Table

```
MAJOR CENTRAL BANKS COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Central Bank         Currency   Policy Rate   RTGS System    CBDC Status │
    │   ──────────────────────────────────────────────────────────────────────── │
    │   Federal Reserve      USD        5.25-5.50%    Fedwire        In research │
    │   (USA)                            (as of 2024)                 (Project ) │
    │                                                                             │
    │   European Central     EUR         4.50%        TARGET2       Digital Euro │
    │   Bank (EU)                                                   (in progress)│
    │                                                                             │
    │   Bank of England      GBP         5.25%        CHAPS         Digital Pound│
    │   (UK)                                                       (in progress)│
    │                                                                             │
    │   Bank of Japan        JPY        -0.10%        BOJ-NET       Digital Yen  │
    │   (Japan)                                                      (in progress)│
    │                                                                             │
    │   People's Bank of     CNY         3.45%        CNAPS         e-CNY        │
    │   China (PRC)                                                   (live pilot)│
    │                                                                             │
    │   Swiss National       CHF         1.75%        SIC5          Project Helvetia│
    │   Bank (Switzerland)                                              (in progress)│
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Payment Systems Operated by Central Banks

### Real-Time Gross Settlement (RTGS) Systems

```
RTGS SYSTEM ARCHITECTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                      ┌─────────────────────────┐                           │
    │                      │    Central Bank RTGS    │                           │
    │                      │         System          │                           │
    │                      │                         │                           │
    │                      │  ┌─────┐    ┌─────┐     │                           │
    │                      │  │Ledger│    │Queue │     │                           │
    │                      │  └──┬──┘    └──┬──┘     │                           │
    │                      │     │          │        │                           │
    │                      │  ┌──┴──────────┴──┐     │                           │
    │                      │  │Settlement Engine│     │                           │
    │                      │  └────────┬────────┘     │                           │
    │                      │           │              │                           │
    │                      └───────────┼──────────────┘                           │
    │                                  │                                           │
    │          ┌───────────┬───────────┼───────────┬───────────┐                 │
    │          │           │           │           │           │                 │
    │          ▼           ▼           ▼           ▼           ▼                 │
    │    ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐        │
    │    │  Bank A  │ │  Bank B  │ │  Bank C  │ │  Bank D  │ │  Bank E  │        │
    │    │ (Reserve │ │ (Reserve │ │ (Reserve │ │ (Reserve │ │ (Reserve │        │
    │    │ Account) │ │ Account) │ │ Account) │ │ Account) │ │ Account) │        │
    │    └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘        │
    │                                                                             │
    │                                                                             │
    │   Key Features:                                                            │
    │   ├── Each payment settled individually (not netted)                       │
    │   ├── Final and irrevocable settlement                                     │
    │   ├── Central bank money (risk-free settlement asset)                      │
    │   ├── Intraday liquidity provided by central bank                          │
    │   └── Typically handles large-value, time-critical payments               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    MAJOR RTGS SYSTEMS SPECIFICATIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   System      Operator      Daily Volume     Settlement     Operating      │
    │                            (USD equivalent)    Asset         Hours         │
    │   ──────────────────────────────────────────────────────────────────────── │
    │   Fedwire     Federal        ~$2.5 trillion   Central bank   22 hours      │
    │              Reserve                         reserves        (US)         │
    │                                                                             │
    │   TARGET2     ECB/Eurosystem ~$2.0 trillion   Central bank   24/7 for      │
    │                                               reserves        some ops     │
    │                                                                             │
    │   CHAPS       Bank of        ~$500 billion    Central bank   6:00-18:00    │
    │              England                         reserves        (UK time)    │
    │                                                                             │
    │   BOJ-NET     Bank of        ~$400 billion    Central bank   9:00-17:00    │
    │              Japan                           reserves        (JST)        │
    │                                                                             │
    │   CNAPS       People's       ~$5 trillion     Central bank   8:30-17:00    │
    │              Bank of China                    reserves        (CST)       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Monetary Policy Implementation

### Policy Tools and Mechanisms

```
MONETARY POLICY TOOLKIT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TOOL                     MECHANISM                    CURRENT USAGE      │
    │   ──────────────────────────────────────────────────────────────────────── │
    │                                                                             │
    │   Policy Rate             Interest on reserve         Primary tool        │
    │   (Federal Funds Rate,    balances (IORB)             for price stability │
    │    Main Refinancing Rate,  overnight reverse         │
    │    Bank Rate)              repurchase agreements      │
    │                                                                             │
    │   Open Market             Buy/sell government        Daily operations     │
    │   Operations (OMO)         securities to adjust       to manage reserves  │
    │                           liquidity                                        │
    │                                                                             │
    │   Reserve                 Minimum reserves           Less common         │
    │   Requirements            banks must hold             (zero in UK, Canada)│
    │                                                                             │
    │   Standing Facilities     Deposit and lending        Corridor for         │
    │                           facilities at policy       market rates         │
    │                           rate ± spread                                    │
    │                                                                             │
    │   Quantitative            Large-scale asset          Used during          │
    │   Easing (QE)             purchases (bonds,          crises (2008, 2020)  │
    │                           MBS) to lower long-                             │
    │                           term rates                                       │
    │                                                                             │
    │   Forward Guidance        Communication of           Shape market         │
    │                           future policy path         expectations         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    INTEREST RATE CORRIDOR SYSTEM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Interest Rate                                                            │
    │        ▲                                                                   │
    │        │                                                                   │
    │   Rate_Lending ─────────────────────────────────────  Standing Lending    │
    │        │                                           ╱   Facility (ceiling)  │
    │        │                                          ╱                        │
    │   Rate_Policy ──────────────────────────────────●───────────────────────  │
    │        │                                        │ ╲      Policy Rate        │
    │        │                                        │  ╲   (target)            │
    │        │                                        │   ╲                       │
    │   Rate_Deposit ──────────────────────────────────────●──────────────────  │
    │        │                                                 ╲  Standing Deposit│
    │        │                                                  ╲ Facility (floor)│
    │        │                                                   ╲                │
    │        │                                                    ╲               │
    │        └────────────────────────────────────────────────────────► Time    │
    │                                                                             │
    │                                                                             │
    │   Market interest rates trade within corridor formed by:                   │
    │   ├── Deposit facility rate (floor) — banks can park excess reserves      │
    │   ├── Lending facility rate (ceiling) — banks can borrow against collateral│
    │   └── Width of corridor typically 50-100 basis points                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Lender of Last Resort (LOLR) Function

### Discount Window Operations

```
LENDER OF LAST RESORT FRAMEWORK

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BAGEHOT'S PRINCIPLE (1873):                                              │
    │   "Lend freely at a penalty rate against good collateral"                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   ELIGIBILITY CRITERIA:                                            │   │
    │   │   ├── Solvent but illiquid (not insolvent)                         │   │
    │   │   ├── Good collateral (government bonds, high-quality assets)      │   │
    │   │   ├── Penalty rate above normal market rate                        │   │
    │   │   └── Discretionary (no automatic right)                           │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   DISCOUNT WINDOW TYPES:                                                   │
    │                                                                             │
    │   Primary Credit (Federal Reserve):                                       │
    │   ├── For financially sound institutions                                  │
    │   ├── No questions asked for first 90 days                               │
    │   ├── Rate = policy rate + 0.50% (penalty)                               │
    │   └── Overnight to 90-day terms                                          │
    │                                                                             │
    │   Secondary Credit:                                                        │
    │   ├── For institutions not qualifying for primary                         │
    │   ├── Higher penalty rate (policy rate + 1.00%)                          │
    │   └── Subject to greater restrictions                                    │
    │                                                                             │
    │   Seasonal Credit:                                                         │
    │   ├── For smaller institutions with seasonal patterns                    │
    │   ├── Rate = average of selected market rates                            │
    │   └── Up to 9 months                                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Reserve Management and Balance Sheet

### Central Bank Balance Sheet Structure

```
CENTRAL BANK BALANCE SHEET

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ASSETS                                LIABILITIES                        │
    │   ───────────────────────────          ───────────────────────────         │
    │                                         │                                   │
    │   Government Securities                 Currency in Circulation            │
    │   (Treasury bonds, bills)               (Banknotes and coins)              │
    │                                         │                                   │
    │   Foreign Exchange Reserves             Reserve Balances                   │
    │   (Foreign currencies, gold, SDR)       (Bank deposits at central bank)    │
    │                                         │                                   │
    │   Loans to Banks                        Government Deposits                │
    │   (Discount window, repo)               (Treasury accounts)                │
    │                                         │                                   │
    │   Other Assets                          Other Liabilities                  │
    │   (Emergency lending,                  (Capital accounts, IMF)            │
    │    crisis facilities)                                                       │
    │                                                                             │
    │   ───────────────────────────          ───────────────────────────         │
    │   TOTAL ASSETS           =            TOTAL LIABILITIES                    │
    │                                                                             │
    │                                                                             │
    │   TYPICAL FEDERAL RESERVE BALANCE SHEET (simplified):                      │
    │                                                                             │
    │   Assets:                                                                  │
    │   ├── US Treasury securities: ~$5 trillion                                 │
    │   ├── Mortgage-backed securities: ~$2.5 trillion                          │
    │   └── Other assets: ~$0.5 trillion                                        │
    │                                                                             │
    │   Liabilities:                                                             │
    │   ├── Currency in circulation: ~$2.3 trillion                              │
    │   ├── Reserve balances: ~$3.5 trillion                                    │
    │   ├── Reverse repo balances: ~$1.5 trillion                               │
    │   └── Other: ~$0.7 trillion                                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    RESERVE REQUIREMENT FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FORMULA:                                                                 │
    │                                                                             │
    │   Required Reserves = Reserve Requirement Ratio × Transaction Deposits     │
    │                                                                             │
    │   EXAMPLE (if ratio = 10%):                                                │
    │                                                                             │
    │   Transaction deposits = $100 million                                      │
    │   Required reserves   = 0.10 × $100 million = $10 million                  │
    │                                                                             │
    │   Excess reserves = Actual reserves - Required reserves                   │
    │                                                                             │
    │   Money multiplier (simple model):                                         │
    │                                                                             │
    │   Money Multiplier = 1 / Reserve Requirement Ratio                         │
    │                                                                             │
    │   If ratio = 10%: Multiplier = 1 / 0.10 = 10                               │
    │                                                                             │
    │   Total money creation = Initial deposit × Multiplier                      │
    │                                                                             │
    │   EXAMPLE: $1 million deposit → up to $10 million money supply             │
    │                                                                             │
    │   NOTE: Many central banks (Canada, UK, Australia) have zero reserves     │
    │         and use interest on reserves as primary tool.                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Central Bank Digital Currency (CBDC)

### CBDC Framework and Design

```
CBDC ARCHITECTURE TYPES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ARCHITECTURE PATTERNS:                                                   │
    │                                                                             │
    │   1. DIRECT CBDC (Retail)                                                 │
    │      ┌────────────────────────────────────────────────────────────┐        │
    │      │  Central Bank ──► Public (individuals, businesses)        │        │
    │      │  Central bank holds all accounts and processes payments    │        │
    │      │  Example: No commercial bank intermediation               │        │
    │      └────────────────────────────────────────────────────────────┘        │
    │                                                                             │
    │   2. INDIRECT CBDC (Two-tier)                                              │
    │      ┌────────────────────────────────────────────────────────────┐        │
    │      │  Central Bank ──► Commercial Banks ──► Public              │        │
    │      │  Central bank issues wholesale CBDC to banks               │        │
    │      │  Banks distribute retail CBDC to public                    │        │
    │      │  Example: Most current proposals (China, Eurozone)         │        │
    │      └────────────────────────────────────────────────────────────┘        │
    │                                                                             │
    │   3. HYBRID CBDC                                                           │
    │      ┌────────────────────────────────────────────────────────────┐        │
    │      │  Central Bank handles wholesale and settlement             │        │
    │      │  Private intermediaries handle customer-facing services     │        │
    │      │  Central bank can see all transactions (privacy concerns)   │        │
    │      └────────────────────────────────────────────────────────────┘        │
    │                                                                             │
    │                                                                             │
    │   CBDC DESIGN DIMENSIONS:                                                  │
    │                                                                             │
    │   ┌───────────────────────────────────────────────────────────────────┐     │
    │   │  DIMENSION              OPTIONS                                   │     │
    │   │  ─────────────────────────────────────────────────────────────── │     │
    │   │  Access                Account-based vs Token-based              │     │
    │   │  Intermediation        Direct vs Indirect vs Hybrid              │     │
    │   │  Remuneration          Interest-bearing vs Zero interest         │     │
    │   │  Anonymity             Anonymous vs Identified vs Tiered         │     │
    │   │  Limits                None vs Transaction vs Balance caps       │     │
    │   │  Technology            DLT vs Traditional centralized ledger     │     │
    │   │  Cross-border          Compatible vs Proprietary                 │     │
    │   └───────────────────────────────────────────────────────────────────┘     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    GLOBAL CBDC STATUS (2024-2025)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STATUS               COUNTRIES / PROJECTS                                │
    │   ──────────────────────────────────────────────────────────────────────── │
    │                                                                             │
    │   LIVE (Full launch)   Bahamas (Sand Dollar), Nigeria (eNaira),            │
    │                        Jamaica (JAM-DEX), Eastern Caribbean (DCash)        │
    │                                                                             │
    │   PILOT (Large scale)  China (e-CNY - 260M users), India (e-Rupee),        │
    │                        Brazil (Drex), Russia (Digital Ruble)               │
    │                                                                             │
    │   PILOT (Wholesale)    Switzerland (Project Helvetia), Singapore         │
    │                        (Project Ubin), France (wCBDC experiments)          │
    │                                                                             │
    │   IN PROGRESS          Eurozone (Digital Euro), UK (Digital Pound),        │
    │                        USA (Project Cedar), Japan, South Korea            │
    │                                                                             │
    │   RESEARCH             Canada, Australia, Sweden (e-krona),               │
    │                        Israel, Norway                                      │
    │                                                                             │
    │   NO PLANS / PAUSED    Germany (prefers digital euro), Ecuador (ended),   │
    │                        Finland (no need), Senegal (ended)                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Cross-Border Central Bank Cooperation

### Bilateral and Multilateral Arrangements

```
CENTRAL BANK COOPERATION FRAMEWORKS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CURRENCY SWAP LINES:                                                     │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Two central banks agree to exchange currencies to provide         │   │
    │   │  liquidity in times of stress.                                     │   │
    │   │                                                                     │   │
    │   │  Federal Reserve standing swap lines:                              │   │
    │   │  ├── Bank of Canada (CAD)                                          │   │
    │   │  ├── Bank of England (GBP)                                         │   │
    │   │  ├── European Central Bank (EUR)                                   │   │
    │   │  ├── Bank of Japan (JPY)                                           │   │
    │   │  ├── Swiss National Bank (CHF)                                     │   │
    │   │  └── Others (Mexico, Brazil, Korea, Singapore - temporary)        │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   MULTILATERAL PLATFORMS:                                                  │
    │                                                                             │
    │   mBridge (BIS Innovation Hub):                                            │
    │   ├── Participants: China, Hong Kong, Thailand, UAE, Saudi Arabia        │
    │   ├── Wholesale CBDC platform for cross-border payments                   │
    │   ├── DLT-based, reduces correspondent banking costs                      │
    │   └── Minimum viable product launched 2024                               │
    │                                                                             │
    │   Project Agorá (BIS, 7 central banks):                                   │
    │   ├── Bank of France, Bank of Japan, Bank of Korea, Bank of Mexico       │
    │   ├── Swiss National Bank, Bank of England, Federal Reserve New York     │
    │   ├── Tokenized commercial bank deposits + wholesale CBDC                │
    │   └── Improves cross-border payment speed and transparency               │
    │                                                                             │
    │   Project Nexus (BIS, 4 central banks):                                   │
    │   ├── Malaysia, Philippines, Singapore, Thailand, India (2024)           │
    │   ├── Links domestic fast payment systems                                 │
    │   └── Enables instant cross-border retail payments                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Oversight and Standards

### International Frameworks

```
CENTRAL BANK OVERSIGHT FRAMEWORKS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CPMI (Committee on Payments and Market Infrastructures):                │
    │   ├── Hosted by Bank for International Settlements (BIS)                  │
    │   ├── 28 member central banks                                             │
    │   ├── Sets standards for payment and settlement systems                   │
    │   └── Publishes PFMI (Principles for Financial Market Infrastructures)   │
    │                                                                             │
    │                                                                             │
    │   PFMI - KEY PRINCIPLES FOR CENTRAL BANKS:                                 │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  PRINCIPLE                    REQUIREMENT                           │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  Principle 1: Legal basis     FMI should have solid legal          │   │
    │   │                               foundation in all jurisdictions      │   │
    │   │                                                                     │   │
    │   │  Principle 2: Governance      Clear, transparent governance        │   │
    │   │                               arrangements                          │   │
    │   │                                                                     │   │
    │   │  Principle 3: Risk management Framework to manage credit,          │   │
    │   │                               liquidity, operational risks         │   │
    │   │                                                                     │   │
    │   │  Principle 4: Credit risk     Measure and cover credit exposures   │   │
    │   │                                                                     │   │
    │   │  Principle 5: Collateral      Low-risk, liquid collateral          │   │
    │   │                                                                     │   │
    │   │  Principle 6: Margin          Risk-based margin requirements       │   │
    │   │                                                                     │   │
    │   │  Principle 7: Liquidity risk  Sufficient liquid resources          │   │
    │   │                                                                     │   │
    │   │  Principle 8: Settlement      Final, timely settlement             │   │
    │   │                                                                     │   │
    │   │  Principle 9: Money settlements Use central bank money where      │   │
    │   │                               possible                              │   │
    │   │                                                                     │   │
    │   │  Principle 10: Physical       Clarify settlement finality          │   │
    │   │              deliveries                                             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Operational Risk and Resilience

### Business Continuity and Cyber Security

```
CENTRAL BANK RESILIENCE REQUIREMENTS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BUSINESS CONTINUITY OBJECTIVES:                                          │
    │                                                                             │
    │   Recovery Time Objective (RTO): < 2 hours for critical systems            │
    │   Recovery Point Objective (RPO): < 5 minutes data loss                    │
    │   Geographic redundancy: Minimum 2 data centers > 50 km apart              │
    │   Annual testing: Full failover drills (minimum 2x per year)              │
    │                                                                             │
    │                                                                             │
    │   CYBER RESILIENCE FRAMEWORK:                                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LAYER                  CONTROLS                                    │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  Identity Management    Multi-factor authentication for all        │   │
    │   │                        privileged access                           │   │
    │   │                                                                     │   │
    │   │  Network Security       Air-gapped backup systems                  │   │
    │   │                        Encrypted communication (TLS 1.3+)          │   │
    │   │                        DDoS protection (multi-terabit capacity)    │   │
    │   │                                                                     │   │
    │   │  Application Security   Regular penetration testing                │   │
    │   │                        Bug bounty programs                         │   │
    │   │                        Secure software development lifecycle       │   │
    │   │                                                                     │   │
    │   │  Data Protection        Encryption at rest (AES-256)               │   │
    │   │                        Encryption in transit (TLS)                 │   │
    │   │                        Hardware security modules (HSMs)            │   │
    │   │                                                                     │   │
    │   │  Monitoring             SIEM with real-time alerting               │   │
    │   │                        24/7 security operations center (SOC)       │   │
    │   │                        Threat hunting and intelligence             │   │
    │   │                                                                     │   │
    │   │  Recovery               Offline backups (air-gapped)               │   │
    │   │                        Manual override capabilities                │   │
    │   │                        Paper-based fallback procedures             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Central Bank Communications

### Forward Guidance and Market Impact

```
FORWARD GUIDANCE FRAMEWORK

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TYPES OF FORWARD GUIDANCE:                                               │
    │                                                                             │
    │   1. Calendar-based:                                                        │
    │      "Policy rate will remain at current level until Q2 2026"             │
    │                                                                             │
    │   2. State-based (outcome):                                                 │
    │      "Rates will not increase until inflation sustainably reaches 2%"     │
    │                                                                             │
    │   3. State-based (threshold):                                               │
    │      "Asset purchases will continue until unemployment falls below 6.5%"  │
    │                                                                             │
    │   4. Open-ended:                                                            │
    │      "Policy will remain accommodative for an extended period"            │
    │                                                                             │
    │                                                                             │
    │   COMMUNICATION CHANNELS:                                                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CHANNEL                    FREQUENCY              AUDIENCE         │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  Monetary Policy Statement  6-8 times per year    Public, markets  │   │
    │   │  Press Conference            After each meeting    Media, public    │   │
    │   │  Meeting Minutes             3 weeks after         Markets, analysts│   │
    │   │  Quarterly Report           4 times per year       Public           │   │
    │   │  Speeches by officials      Ongoing (monthly)      Markets, experts │   │
    │   │  Economic Projections       4 times per year       Markets          │   │
    │   │  (dot plots)                                                        │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

| Formula / Concept | Purpose |
|------------------|---------|
| Money Multiplier = 1 / Reserve Requirement Ratio | Maximum potential money creation |
| Required Reserves = RR Ratio × Transaction Deposits | Minimum reserves a bank must hold |
| Excess Reserves = Actual Reserves - Required Reserves | Lendable funds beyond requirements |
| Policy Rate Corridor = Lending Rate - Deposit Rate | Width of interest rate band |
| Real Interest Rate = Nominal Rate - Inflation Rate | Inflation-adjusted return |
| Quantity Theory: MV = PQ | Money supply × Velocity = Price × Output |
| Taylor Rule: i = r* + π + 0.5(π - π*) + 0.5(y - y*) | Policy rate guidance formula |
| Reserve Balance = Assets - Currency - Other Liabilities | Central bank liquidity calculation |
| Discount Window Penalty = Policy Rate + Spread (0.50% for primary) | Cost of LOLR borrowing |

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