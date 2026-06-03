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
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                        CENTRAL BANK                                 │   │
    │   │                             │                                       │   │
    │   │         ┌───────────────────┼───────────────────┐                   │   │
    │   │         │                   │                   │                   │   │
    │   │         ▼                   ▼                   ▼                   │   │
    │   │   ┌──────────┐       ┌──────────┐       ┌──────────┐                │   │
    │   │   │ Monetary │       │ Currency │       │ Payment  │                │   │
    │   │   │ Policy   │       │ Issuance │       │ Systems  │                │   │
    │   │   └────┬─────┘       └────┬─────┘       └────┬─────┘                │   │
    │   │        │                  │                  │                      │   │
    │   │        └──────────────────┼──────────────────┘                      │   │
    │   │                           │                                         │   │
    │   │         ┌─────────────────┼─────────────────┐                       │   │
    │   │         │                 │                 │                       │   │
    │   │         ▼                 ▼                 ▼                       │   │
    │   │   ┌──────────┐       ┌──────────┐       ┌──────────┐                │   │
    │   │   │ Lender of│       │ Reserve  │       │ Financial│                │   │
    │   │   │ Last     │       │ Mgt      │       │ Stability│                │   │
    │   │   │ Resort   │       │          │       │          │                │   │
    │   │   └──────────┘       └──────────┘       └──────────┘                │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   FUNCTION BREAKDOWN:                                                       │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Monetary Policy                                                    │   │
    │   │  ├── Price stability (inflation targeting)                          │   │
    │   │  ├── Interest rate setting (policy rate)                            │   │
    │   │  ├── Open market operations (buy/sell securities)                   │   │
    │   │  ├── Reserve requirements                                           │   │
    │   │  └── Quantitative easing (asset purchases)                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Currency Issuance                                                  │   │
    │   │  ├── Sole right to issue banknotes and coins                        │   │
    │   │  ├── Maintain public confidence in currency                         │   │
    │   │  ├── Manage currency supply                                         │   │
    │   │  └── Combat counterfeiting                                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Payment System Oversight                                           │   │
    │   │  ├── Operate RTGS systems (Fedwire, TARGET2, CHAPS)                 │   │
    │   │  ├── Oversee retail payment systems                                 │   │
    │   │  ├── Ensure settlement finality                                     │   │
    │   │  └── Reduce systemic risk                                           │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Lender of Last Resort                                              │   │
    │   │  ├── Provide emergency liquidity to banks                           │   │
    │   │  ├── Prevent bank runs                                              │   │
    │   │  ├── Maintain financial stability                                   │   │
    │   │  └── Operate discount window                                        │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Foreign Exchange Reserve Management                                │   │
    │   │  ├── Hold and manage foreign currency reserves                      │   │
    │   │  ├── Intervene in currency markets                                  │   │
    │   │  ├── Maintain exchange rate stability                               │   │
    │   │  └── Support international trade                                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Monetary Policy Transmission Mechanism

```
MONETARY POLICY TRANSMISSION CHAIN

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CENTRAL BANK ACTION                                                       │
    │        │                                                                    │
    │        ▼                                                                    │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Policy Rate Change                                                 │   │
    │   │  Open Market Operation                                              │   │
    │   │  Reserve Requirement Adjustment                                     │   │
    │   │  Quantitative Easing                                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                    │
    │        ▼                                                                    │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  INTERBANK MARKET                                                   │   │
    │   │                                                                     │   │
    │   │  ┌──────────┐    ┌──────────┐    ┌──────────┐                       │   │
    │   │  │ Bank A   │◄──►│ Bank B   │◄──►│ Bank C   │                       │   │
    │   │  └──────────┘    └──────────┘    └──────────┘                       │   │
    │   │        ▲               ▲               ▲                            │   │
    │   │        └───────────────┼───────────────┘                            │   │
    │   │                    Rates change                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                    │
    │        ▼                                                                    │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  COMMERCIAL BANK RESPONSE                                           │   │
    │   │                                                                     │   │
    │   │  Deposit Rates ──────────────────► Savings behavior                 │   │
    │   │  Lending Rates  ──────────────────► Loan demand                     │   │
    │   │  Credit Standards ────────────────► Loan approval rates             │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                    │
    │        ▼                                                                    │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  BUSINESS & CONSUMER RESPONSE                                       │   │
    │   │                                                                     │   │
    │   │  Investment ──────────────────────► Capital spending                │   │
    │   │  Consumption ─────────────────────► Durable goods purchases         │   │
    │   │  Housing ─────────────────────────► Mortgage demand                 │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                    │
    │        ▼                                                                    │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  ECONOMIC OUTCOMES                                                  │   │
    │   │                                                                     │   │
    │   │  GDP Growth ◄──────────────────────► Inflation Rate                 │   │
    │   │  Employment ◄──────────────────────► Asset Prices                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    TRANSMISSION CHANNELS TABLE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Channel              │ Mechanism                         │ Lag Time       │
    │   ─────────────────────│───────────────────────────────────│──────────────  │
    │   Interest rate        │ Policy rate → bank rates →        │ 6-12 months    │
    │   channel              │ spending/investment               │                │
    │   ─────────────────────│───────────────────────────────────│──────────────  │
    │   Credit channel       │ Bank lending capacity → loan      │ 3-9 months     │
    │                        │ availability                      │                │
    │   ─────────────────────│───────────────────────────────────│──────────────  │
    │   Exchange rate        │ Interest differential → currency  │ Immediate      │
    │   channel              │ value → net exports               │                │
    │   ─────────────────────│───────────────────────────────────│──────────────  │
    │   Asset price channel  │ Discount rates → asset values →   │ 3-6 months     │
    │                        │ wealth effect                     │                │
    │   ─────────────────────│───────────────────────────────────│──────────────  │
    │   Expectations channel │ Forward guidance → market         │ Immediate      │
    │                        │ expectations → current behavior   │                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Major Central Banks Overview

### Central Bank Comparison

```
MAJOR CENTRAL BANKS COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Federal Reserve (USA)                                                     │
    │   ├── Currency: USD                                                         │
    │   ├── Policy Rate: 5.25-5.50% (as of 2024)                                  │
    │   ├── RTGS System: Fedwire                                                  │
    │   ├── CBDC Status: In research (Project Cedar)                              │
    │   └── Unique: Dual mandate (price stability + maximum employment)           │
    │                                                                             │
    │   European Central Bank (EU)                                                │
    │   ├── Currency: EUR                                                         │
    │   ├── Policy Rate: 4.50%                                                    │
    │   ├── RTGS System: TARGET2                                                  │
    │   ├── CBDC Status: Digital Euro (in progress)                               │
    │   └── Unique: Serves 20 eurozone countries                                  │
    │                                                                             │
    │   Bank of England (UK)                                                      │
    │   ├── Currency: GBP                                                         │
    │   ├── Policy Rate: 5.25%                                                    │
    │   ├── RTGS System: CHAPS                                                    │
    │   ├── CBDC Status: Digital Pound (in progress)                              │
    │   └── Unique: Oldest central bank (1694)                                    │
    │                                                                             │
    │   Bank of Japan (Japan)                                                     │
    │   ├── Currency: JPY                                                         │
    │   ├── Policy Rate: -0.10%                                                   │
    │   ├── RTGS System: BOJ-NET                                                  │
    │   ├── CBDC Status: Digital Yen (in progress)                                │
    │   └── Unique: Negative interest rate policy                                 │
    │                                                                             │
    │   People's Bank of China (PRC)                                              │
    │   ├── Currency: CNY                                                         │
    │   ├── Policy Rate: 3.45%                                                    │
    │   ├── RTGS System: CNAPS                                                    │
    │   ├── CBDC Status: e-CNY (live pilot, 260M users)                           │
    │   └── Unique: Most advanced CBDC deployment                                 │
    │                                                                             │
    │   Swiss National Bank (Switzerland)                                         │
    │   ├── Currency: CHF                                                         │
    │   ├── Policy Rate: 1.75%                                                    │
    │   ├── RTGS System: SIC5                                                     │
    │   ├── CBDC Status: Project Helvetia (wholesale pilot)                       │
    │   └── Unique: First major wholesale CBDC pilot                              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Payment Systems Operated by Central Banks

### Real-Time Gross Settlement (RTGS) System Architecture

```
RTGS SYSTEM ARCHITECTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                      ┌─────────────────────────────────────┐                │
    │                      │         CENTRAL BANK RTGS           │                │
    │                      │                                     │                │
    │                      │  ┌─────────┐        ┌─────────┐     │                │
    │                      │  │ Reserve │        │ Payment │     │                │
    │                      │  │ Ledger  │        │  Queue  │     │                │
    │                      │  └────┬────┘        └────┬────┘     │                │
    │                      │       │                  │          │                │
    │                      │       └────────┬─────────┘          │                │
    │                      │                │                    │                │
    │                      │       ┌────────┴────────┐           │                │
    │                      │       │  Settlement     │           │                │
    │                      │       │    Engine       │           │                │
    │                      │       └────────┬────────┘           │                │
    │                      │                │                    │                │
    │                      └────────────────┼────────────────────┘                │
    │                                       │                                     │
    │         ┌─────────────┬───────────────┼───────────────┬─────────────┐       │
    │         │             │               │               │             │       │
    │         ▼             ▼               ▼               ▼             ▼       │
    │   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐  │
    │   │  Bank A  │   │  Bank B  │   │  Bank C  │   │  Bank D  │   │  Bank E  │  │
    │   │ Reserve  │   │ Reserve  │   │ Reserve  │   │ Reserve  │   │ Reserve  │  │
    │   │ Account  │   │ Account  │   │ Account  │   │ Account  │   │ Account  │  │
    │   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘  │
    │                                                                             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  KEY FEATURES:                                                      │   │
    │   │  ├── Each payment settled individually (not netted)                 │   │
    │   │  ├── Final and irrevocable settlement                               │   │
    │   │  ├── Central bank money (risk-free settlement asset)                │   │
    │   │  ├── Intraday liquidity provided by central bank                    │   │
    │   │  └── Handles large-value, time-critical payments                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    LIQUIDITY SAVING MECHANISM (LSM)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   WITHOUT LSM                      │ WITH LSM                               │
    │                                    │                                        │
    │   Payment A ──┐                    │ Payment A ──┐                          │
    │   Payment B ──┼── Queue ──► Settle │ Payment B ──┼── Queue ──┬── Offset ──┐ │
    │   Payment C ──┘                    │ Payment C ──┘           │            │ │
    │                                    │                         │            ▼ │
    │   Requires: 3 units of liquidity   │                         │    ┌─────────────┐
    │                                    │                         │    │   Net       │
    │                                    │                         └───►│ Settlement  │
    │                                    │                              │  (1 unit)   │
    │                                    │                              └─────────────┘
    │                                                                             │
    │   LSM MECHANISM:                                                            │
    │   ├── Payment queuing and prioritization                                    │
    │   ├── Bilateral and multilateral offsetting                                 │
    │   ├── Partial settlement using available liquidity                          │
    │   └── Reduces liquidity needs by 40-60%                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    MAJOR RTGS SYSTEMS SPECIFICATIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   System    │ Operator        │ Daily Volume   │ Hours       │ LSM          │
    │   ──────────│─────────────────│────────────────│─────────────│────────────  │
    │   Fedwire   │ Federal Reserve │ ~$2.5 trillion │ 22 hours    │ Yes          │
    │   ──────────│─────────────────│────────────────│─────────────│────────────  │
    │   TARGET2   │ ECB/Eurosystem  │ ~$2.0 trillion │ 24/7 (some) │ Yes          │
    │   ──────────│─────────────────│────────────────│─────────────│────────────  │
    │   CHAPS     │ Bank of England │ ~$500 billion  │ 6:00-18:00  │ Yes          │
    │   ──────────│─────────────────│────────────────│─────────────│────────────  │
    │   BOJ-NET   │ Bank of Japan   │ ~$400 billion  │ 9:00-17:00  │ Yes          │
    │   ──────────│─────────────────│────────────────│─────────────│────────────  │
    │   CNAPS     │ PBOC            │ ~$5 trillion   │ 8:30-17:00  │ Yes          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Monetary Policy Implementation

### Policy Tools and Mechanisms

```
MONETARY POLICY TOOLKIT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                        POLICY RATE                                  │   │
    │   │                                                                     │   │
    │   │   Interest on Reserve Balances (IORB)                               │   │
    │   │   Overnight Reverse Repurchase (ON RRP)                             │   │
    │   │                                                                     │   │
    │   │   Effect: Primary tool for price stability                          │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                      │                                      │
    │                                      ▼                                      │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                    OPEN MARKET OPERATIONS (OMO)                     │   │
    │   │                                                                     │   │
    │   │   ┌──────────────┐          ┌──────────────┐                        │   │
    │   │   │ Central Bank │─────────►│  Commercial  │                        │   │
    │   │   │              │◄─────────│    Banks     │                        │   │
    │   │   └──────────────┘          └──────────────┘                        │   │
    │   │        │                           │                                │   │
    │   │        ▼                           ▼                                │   │
    │   │   Buy/Sell Securities        Reserves Increase/Decrease             │   │
    │   │                                                                     │   │
    │   │   Effect: Daily reserve management                                  │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                      │                                      │
    │                                      ▼                                      │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                    STANDING FACILITIES                              │   │
    │   │                                                                     │   │
    │   │   Deposit Facility (Floor)     Lending Facility (Ceiling)           │   │
    │   │   Rate = Policy - Spread       Rate = Policy + Spread               │   │
    │   │                                                                     │   │
    │   │   Effect: Creates interest rate corridor                            │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                      │                                      │
    │                                      ▼                                      │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                  QUANTITATIVE EASING (QE)                           │   │
    │   │                                                                     │   │
    │   │   Central Bank ──► Buys Bonds ──► Injects Liquidity                 │   │
    │   │                                                                     │   │
    │   │   Effect: Lowers long-term rates during crises                      │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                      │                                      │
    │                                      ▼                                      │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                       FORWARD GUIDANCE                              │   │
    │   │                                                                     │   │
    │   │   "Policy rate will remain at current level until conditions met"   │   │
    │   │                                                                     │   │
    │   │   Effect: Shapes market expectations                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Interest Rate Corridor System

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                                             │
│   Interest Rate                                                             │
│         ▲                                                                   │
│         │                                                                   │
│   5.00% ┼ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ Ceiling   │
│         │               \                                                   │
│   4.75% ┼                \    Demand for Reserves                           │
│         │                 \                                                 │
│   4.50% ┼ ─ ─ ─ ─ ─ ─ ─ ─  \  ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ Target    │
│         │                   \                                               │
│   4.25% ┼                    \                                              │
│         │                     \                                             │
│   4.00% ┼ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─  \───────────────────────── ─ ─ ─ ─ Floor     │
│         │                       (Perfectly elastic at floor)                │
│   3.75% ┼                                                                   │
│         │                                                                   │
│         └────────────────────────────────────────────────────────► Quantity │
│                                                                             │
│   ┌─────────────────────────────────────────────────────────────────────┐   │
│   │  CORRIDOR COMPONENTS:                                               │   │
│   │                                                                     │   │
│   │  Lending Facility Rate (Ceiling) = Policy Rate + 0.50%              │   │
│   │  └── Banks can borrow overnight against collateral                  │   │
│   │                                                                     │   │
│   │  Policy Rate (Target) = 4.50%                                       │   │
│   │  └── Announced target for interbank lending                         │   │
│   │                                                                     │   │
│   │  Deposit Facility Rate (Floor) = Policy Rate - 0.50%                │   │
│   │  └── Banks can park excess reserves overnight                       │   │
│   │                                                                     │   │
│   │  Corridor Width = 100 basis points (1.00%)                          │   │
│   └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

## Lender of Last Resort (LOLR) Function

### Discount Window Operations

```
LENDER OF LAST RESORT FRAMEWORK

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BAGEHOT'S PRINCIPLE (1873):                                               │
    │   "Lend freely at a penalty rate against good collateral"                   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   DISTRESSED BANK ──► Central Bank ──► LIQUIDITY PROVIDED           │   │
    │   │        │                    │                    │                  │   │
    │   │        ▼                    ▼                    ▼                  │   │
    │   │   Solvent but           Good              Penalty Rate              │   │
    │   │   Illiquid?            Collateral?        +0.50%                    │   │
    │   │        │                    │                    │                  │   │
    │   │        └────────────┬───────┘                    │                  │   │
    │   │                     ▼                            ▼                  │   │
    │   │                YES + YES ──────────────────► APPROVED               │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   DISCOUNT WINDOW TIERS:                                                    │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  PRIMARY CREDIT                                                     │   │
    │   │  ├── For financially sound institutions                             │   │
    │   │  ├── No questions asked for first 90 days                           │   │
    │   │  ├── Rate = policy rate + 0.50% (penalty)                           │   │
    │   │  └── Overnight to 90-day terms                                      │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  SECONDARY CREDIT                                                   │   │
    │   │  ├── For institutions not qualifying for primary                    │   │
    │   │  ├── Higher penalty rate (policy rate + 1.00%)                      │   │
    │   │  └── Subject to greater restrictions                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  SEASONAL CREDIT                                                    │   │
    │   │  ├── For smaller institutions with seasonal patterns                │   │
    │   │  ├── Rate = average of selected market rates                        │   │
    │   │  └── Up to 9 months                                                 │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    DISCOUNT WINDOW OPERATION FLOW

    ┌────────────────────────────────────────────────┐
    │                                                │
    │   ┌─────────────┐                              │
    │   │  Bank has   │                              │
    │   │  Liquidity  │                              │
    │   │  Shortfall  │                              │
    │   └──────┬──────┘                              │
    │          │                                     │
    │          ▼                                     │
    │   ┌─────────────┐     NO     ┌─────────────┐   │
    │   │  Solvent?   │───────────►│  Denied     │   │
    │   └──────┬──────┘            └─────────────┘   │
    │          │ YES                                 │
    │          ▼                                     │
    │   ┌─────────────┐     NO     ┌─────────────┐   │
    │   │  Eligible   │───────────►│ Secondary   │   │
    │   │  Collateral?│            │  Credit     │   │
    │   └──────┬──────┘            └─────────────┘   │
    │          │ YES                                 │
    │          ▼                                     │
    │   ┌─────────────┐                              │
    │   │  Primary    │                              │
    │   │  Credit     │                              │
    │   │  Approved   │                              │
    │   └──────┬──────┘                              │
    │          │                                     │
    │          ▼                                     │
    │   ┌─────────────┐                              │
    │   │  Liquidity  │                              │
    │   │  Provided   │                              │
    │   └─────────────┘                              │
    │                                                │
    └────────────────────────────────────────────────┘
```

## Reserve Management and Balance Sheet

### Central Bank Balance Sheet Structure

```
CENTRAL BANK BALANCE SHEET

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                         CENTRAL BANK BALANCE SHEET                          │
    │                                                                             │
    │   ┌─────────────────────────────┐   ┌─────────────────────────────┐         │
    │   │          ASSETS             │   │        LIABILITIES          │         │
    │   ├─────────────────────────────┤   ├─────────────────────────────┤         │
    │   │                             │   │                             │         │
    │   │  ┌───────────────────────┐  │   │  ┌───────────────────────┐  │         │
    │   │  │ Government Securities │  │   │  │ Currency in           │  │         │
    │   │  │ (Treasury bonds,      │  │   │  │ Circulation           │  │         │
    │   │  │  bills, MBS)          │  │   │  │ (Banknotes, coins)    │  │         │
    │   │  └───────────────────────┘  │   │  └───────────────────────┘  │         │
    │   │                             │   │                             │         │
    │   │  ┌───────────────────────┐  │   │  ┌───────────────────────┐  │         │
    │   │  │ Foreign Exchange      │  │   │  │ Reserve Balances      │  │         │
    │   │  │ Reserves              │  │   │  │ (Bank deposits at     │  │         │
    │   │  │ (Foreign currencies,  │  │   │  │  central bank)        │  │         │
    │   │  │  gold, SDR)           │  │   │  └───────────────────────┘  │         │
    │   │  └───────────────────────┘  │   │                             │         │
    │   │                             │   │  ┌───────────────────────┐  │         │
    │   │  ┌───────────────────────┐  │   │  │ Government Deposits   │  │         │
    │   │  │ Loans to Banks        │  │   │  │ (Treasury accounts)   │  │         │
    │   │  │ (Discount window,     │  │   │  └───────────────────────┘  │         │
    │   │  │  repo agreements)     │  │   │                             │         │
    │   │  └───────────────────────┘  │   │  ┌───────────────────────┐  │         │
    │   │                             │   │  │ Other Liabilities     │  │         │
    │   │  ┌───────────────────────┐  │   │  │ (Capital accounts,    │  │         │
    │   │  │ Other Assets          │  │   │  │  IMF SDR allocations) │  │         │
    │   │  │ (Emergency lending,   │  │   │  └───────────────────────┘  │         │
    │   │  │  crisis facilities)   │  │   │                             │         │
    │   │  └───────────────────────┘  │   │                             │         │
    │   │                             │   │                             │         │
    │   ├─────────────────────────────┤   ├─────────────────────────────┤         │
    │   │      TOTAL ASSETS           │   │    TOTAL LIABILITIES        │         │
    │   └─────────────────────────────┘   └─────────────────────────────┘         │
    │                                                                             │
    │   BALANCE SHEET IDENTITY: TOTAL ASSETS = TOTAL LIABILITIES                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    TYPICAL FEDERAL RESERVE BALANCE SHEET (simplified)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ASSETS (USD)                        LIABILITIES (USD)                     │
    │   ─────────────────────────────────    ─────────────────────────────────    │
    │                                                                             │
    │   ┌─────────────────────────────┐      ┌─────────────────────────────┐      │
    │   │ US Treasury Securities      │      │ Currency in Circulation     │      │
    │   │ ~$5.0 trillion              │      │ ~$2.3 trillion              │      │
    │   └─────────────────────────────┘      └─────────────────────────────┘      │
    │                                                                             │
    │   ┌─────────────────────────────┐      ┌─────────────────────────────┐      │
    │   │ MBS                         │      │ Reserve Balances            │      │
    │   │ ~$2.5 trillion              │      │ ~$3.5 trillion              │      │
    │   └─────────────────────────────┘      └─────────────────────────────┘      │
    │                                                                             │
    │   ┌─────────────────────────────┐      ┌─────────────────────────────┐      │
    │   │ Other Assets                │      │ Reverse Repo Balances       │      │
    │   │ ~$0.5 trillion              │      │ ~$1.5 trillion              │      │
    │   └─────────────────────────────┘      └─────────────────────────────┘      │
    │                                                                             │
    │   ┌─────────────────────────────┐      ┌─────────────────────────────┐      │
    │   │                             │      │ Other Liabilities           │      │
    │   │                             │      │ ~$0.7 trillion              │      │
    │   │                             │      └─────────────────────────────┘      │
    │   │                             │                                           │
    │   │                             │      ┌─────────────────────────────┐      │
    │   │                             │      │ TOTAL LIABILITIES           │      │
    │   │ TOTAL ASSETS                │      │ ~$8.0 trillion              │      │
    │   │ ~$8.0 trillion              │      │                             │      │
    │   └─────────────────────────────┘      └─────────────────────────────┘      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    MONEY MULTIPLIER MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FORMULA:                                                                  │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Money Multiplier = 1 / Reserve Requirement Ratio                  │   │
    │   │                                                                     │   │
    │   │   Total Money Creation = Initial Deposit × Money Multiplier         │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │   EXAMPLE (Reserve Ratio = 10%):                                            │
    │                                                                             │
    │   Initial Deposit: $1,000                                                   │
    │                                                                             │
    │   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐  │
    │   │   Bank A    │───►│   Bank B    │───►│   Bank C    │───►│     ...     │  │
    │   │             │    │             │    │             │    │             │  │
    │   │ Deposit:    │    │ Deposit:    │    │ Deposit:    │    │             │  │
    │   │ $1,000      │    │ $900        │    │ $810        │    │             │  │
    │   │ Reserve:    │    │ Reserve:    │    │ Reserve:    │    │             │  │
    │   │ $100        │    │ $90         │    │ $81         │    │             │  │
    │   │ Loan: $900  │    │ Loan: $810  │    │ Loan: $729  │    │             │  │
    │   └─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘  │
    │                                                                             │
    │   Total Money Created = $1,000 × 10 = $10,000                               │
    │                                                                             │
    │   NOTE: Many central banks (Canada, UK, Australia) have zero reserve        │
    │         requirements and use interest on reserves as primary tool.          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Central Bank Digital Currency (CBDC)

### CBDC Architecture Types

```
CBDC ARCHITECTURE COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DIRECT CBDC (RETAIL)                                                     │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                        CENTRAL BANK                                 │   │
    │   │                             │                                       │   │
    │   │              ┌──────────────┼──────────────┐                        │   │
    │   │              │              │              │                        │   │
    │   │              ▼              ▼              ▼                        │   │
    │   │         ┌────────┐    ┌────────┐    ┌────────┐                     │   │
    │   │         │Public A│    │Public B│    │Public C│                     │   │
    │   │         └────────┘    └────────┘    └────────┘                     │   │
    │   │                                                                     │   │
    │   │   Central bank holds all accounts and processes payments directly  │   │
    │   │   No commercial bank intermediation                                │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   INDIRECT CBDC (TWO-TIER)                                                 │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                        CENTRAL BANK                                 │   │
    │   │                             │                                       │   │
    │   │              ┌──────────────┼──────────────┐                        │   │
    │   │              │              │              │                        │   │
    │   │              ▼              ▼              ▼                        │   │
    │   │         ┌────────┐    ┌────────┐    ┌────────┐                     │   │
    │   │         │ Bank A │    │ Bank B │    │ Bank C │                     │   │
    │   │         └───┬────┘    └───┬────┘    └───┬────┘                     │   │
    │   │             │             │             │                           │   │
    │   │     ┌───────┼───────┐ ┌───┼───────┐ ┌───┼───────┐                   │   │
    │   │     ▼       ▼       ▼ ▼   ▼       ▼ ▼   ▼       ▼                   │   │
    │   │   ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐          │   │
    │   │   │ P  │ │ P  │ │ P  │ │ P  │ │ P  │ │ P  │ │ P  │ │ P  │          │   │
    │   │   └────┘ └────┘ └────┘ └────┘ └────┘ └────┘ └────┘ └────┘          │   │
    │   │                                                                     │   │
    │   │   Central bank issues wholesale CBDC to banks                      │   │
    │   │   Banks distribute retail CBDC to public                           │   │
    │   │   Most current proposals (China, Eurozone)                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   HYBRID CBDC                                                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   CENTRAL BANK ──────────────────────────────────────────┐          │   │
    │   │        │                                                │          │   │
    │   │        │ Wholesale CBDC                                 │ Oversight│   │
    │   │        ▼                                                ▼          │   │
    │   │   ┌─────────────────────────────────────────────────────────────┐  │   │
    │   │   │                    COMMERCIAL BANKS                         │  │   │
    │   │   │                                                             │  │   │
    │   │   │  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐       │  │   │
    │   │   │  │  Bank   │  │  Bank   │  │  Bank   │  │  Bank   │       │  │   │
    │   │   │  │    A    │  │    B    │  │    C    │  │    D    │       │  │   │
    │   │   │  └────┬────┘  └────┬────┘  └────┬────┘  └────┬────┘       │  │   │
    │   │   │       │            │            │            │             │  │   │
    │   │   │       ▼            ▼            ▼            ▼             │  │   │
    │   │   │    Public       Public        Public        Public          │  │   │
    │   │   └─────────────────────────────────────────────────────────────┘  │   │
    │   │                                                                     │   │
    │   │   Central bank handles wholesale settlement                        │   │
    │   │   Private intermediaries handle customer-facing services           │   │
    │   │   Central bank can see all transactions (privacy concerns)         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    CBDC DESIGN DIMENSIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   DIMENSION              │ OPTIONS                                         │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Access                 │ Account-based ──── Token-based                  │
    │                          │ (identity-linked)   (bearer instrument)         │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Intermediation         │ Direct ──── Indirect ──── Hybrid                │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Remuneration           │ Interest-bearing ──── Zero interest             │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Anonymity              │ Anonymous ──── Tiered ──── Identified           │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Limits                 │ None ──── Transaction ──── Balance caps         │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Technology             │ DLT ──── Traditional centralized ledger         │
    │   ───────────────────────│─────────────────────────────────────────────────│
    │   Cross-border           │ Compatible ──── Proprietary                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    GLOBAL CBDC STATUS (2024-2025)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STATUS               │ COUNTRIES / PROJECTS                              │
    │   ─────────────────────│───────────────────────────────────────────────────│
    │   LIVE (Full launch)   │ Bahamas (Sand Dollar)                             │
    │                        │ Nigeria (eNaira)                                  │
    │                        │ Jamaica (JAM-DEX)                                 │
    │                        │ Eastern Caribbean (DCash)                         │
    │   ─────────────────────│───────────────────────────────────────────────────│
    │   PILOT (Large scale)  │ China (e-CNY - 260M users)                        │
    │                        │ India (e-Rupee)                                   │
    │                        │ Brazil (Drex)                                     │
    │                        │ Russia (Digital Ruble)                            │
    │   ─────────────────────│───────────────────────────────────────────────────│
    │   PILOT (Wholesale)    │ Switzerland (Project Helvetia)                    │
    │                        │ Singapore (Project Ubin)                          │
    │                        │ France (wCBDC experiments)                        │
    │   ─────────────────────│───────────────────────────────────────────────────│
    │   IN PROGRESS          │ Eurozone (Digital Euro)                           │
    │                        │ UK (Digital Pound)                                │
    │                        │ USA (Project Cedar)                               │
    │                        │ Japan, South Korea                                │
    │   ─────────────────────│───────────────────────────────────────────────────│
    │   RESEARCH             │ Canada, Australia, Sweden (e-krona)               │
    │                        │ Israel, Norway                                    │
    │   ─────────────────────│───────────────────────────────────────────────────│
    │   NO PLANS / PAUSED    │ Germany (prefers digital euro)                    │
    │                        │ Ecuador (ended), Finland (no need)                │
    │                        │ Senegal (ended)                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Cross-Border Central Bank Cooperation

### Bilateral and Multilateral Arrangements

```
CURRENCY SWAP LINES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   BILATERAL CURRENCY SWAP ARRANGEMENT                                       │
    │                                                                             │
    │   ┌─────────────────────┐                       ┌─────────────────────┐    │
    │   │    CENTRAL BANK A   │                       │    CENTRAL BANK B   │    │
    │   │        (USD)        │                       │        (EUR)        │    │
    │   │                     │                       │                     │    │
    │   │  ┌───────────────┐  │    Swap Agreement     │  ┌───────────────┐  │    │
    │   │  │ Sends USD     │──┼───────────────────────┼─►│ Receives USD  │  │    │
    │   │  │               │  │                       │  │               │  │    │
    │   │  │ Receives EUR  │◄─┼───────────────────────┼──│ Sends EUR     │  │    │
    │   │  └───────────────┘  │                       │  └───────────────┘  │    │
    │   │                     │                       │                     │    │
    │   └─────────────────────┘                       └─────────────────────┘    │
    │                                                                             │
    │   Federal Reserve Standing Swap Lines:                                     │
    │   ├── Bank of Canada (CAD)                                                 │
    │   ├── Bank of England (GBP)                                                │
    │   ├── European Central Bank (EUR)                                          │
    │   ├── Bank of Japan (JPY)                                                  │
    │   ├── Swiss National Bank (CHF)                                            │
    │   └── Others (Mexico, Brazil, Korea, Singapore - temporary)               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    MULTILATERAL PLATFORMS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   mBridge (BIS Innovation Hub)                                             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   China ──┐                                                         │   │
    │   │   Hong Kong┼──┐                                                     │   │
    │   │   Thailand ┼──┼── DLT Platform ──► Cross-border Settlement         │   │
    │   │   UAE      ┼──┘                                                     │   │
    │   │   Saudi ───┘                                                        │   │
    │   │                                                                     │   │
    │   │   Wholesale CBDC platform for cross-border payments                │   │
    │   │   Reduces correspondent banking costs                               │   │
    │   │   Minimum viable product launched 2024                              │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   Project Nexus (BIS)                                                      │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   Malaysia ──┐                                                      │   │
    │   │   Philippines┼──┐                                                   │   │
    │   │   Singapore  ┼──┼── Link FPS Systems ──► Instant Cross-border      │   │
    │   │   Thailand   ┼──┘                        Retail Payments            │   │
    │   │   India ─────┘                                                      │   │
    │   │                                                                     │   │
    │   │   Links domestic fast payment systems                               │   │
    │   │   Enables instant cross-border retail payments                      │   │
    │   │   Users pay as easily as domestic                                   │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Oversight and Standards

### International Frameworks

```
CPMI AND PFMI FRAMEWORK

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CPMI (Committee on Payments and Market Infrastructures)                  │
    │   │                                                                         │
    │   ├── Hosted by Bank for International Settlements (BIS)                   │
    │   ├── 28 member central banks                                              │
    │   ├── Sets standards for payment and settlement systems                    │
    │   └── Publishes PFMI (Principles for Financial Market Infrastructures)    │
    │                                                                             │
    │                                                                             │
    │   PFMI - 24 PRINCIPLES FOR FMIs                                            │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  PRINCIPLE                     CATEGORY                             │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  1. Legal basis                General organization                │   │
    │   │  2. Governance                  (Principles 1-3)                    │   │
    │   │  3. Risk management                                               │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  4. Credit risk                 Credit & liquidity risk            │   │
    │   │  5. Collateral                   (Principles 4-7)                  │   │
    │   │  6. Margin                                                        │   │
    │   │  7. Liquidity risk                                                │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  8. Settlement finality         Settlement (Principles 8-10)      │   │
    │   │  9. Money settlements                                             │   │
    │   │  10. Physical deliveries                                           │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  11. CSDs (central securities    Central securities depositories  │   │
    │   │       depositories)               (Principles 11-12)              │   │
    │   │  12. Exchange-of-value                                             │   │
    │   │       settlement systems                                           │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  13. Participant-default rules   Default management &             │   │
    │   │  14. Segregation & transfer        operational risk              │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  15. General business risk       Business & operational           │   │
    │   │  16. Custody & investment risks   (Principles 15-17)              │   │
    │   │  17. Operational risk                                              │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  18. Access & participation      Access & efficiency              │   │
    │   │  19. Tiered participation         (Principles 18-20)              │   │
    │   │  20. Efficiency & transparency                                     │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  21. Communication & reporting   Transparency (Principles 21-22)  │   │
    │   │  22. Disclosure                                                   │   │
    │   │  ───────────────────────────────────────────────────────────────── │   │
    │   │  23. Resilience                  Resilience & recovery            │   │
    │   │  24. Recovery & wind-down         (Principles 23-24)              │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Operational Risk and Resilience

### Business Continuity and Cyber Security

```
CENTRAL BANK RESILIENCE ARCHITECTURE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   RESILIENCE LAYERS                                                        │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LAYER 5: RECOVERY                                                  │   │
    │   │  ├── Offline air-gapped backups                                    │   │
    │   │  ├── Manual override capabilities                                  │   │
    │   │  └── Paper-based fallback procedures                               │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                    ▲                                       │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LAYER 4: MONITORING                                                │   │
    │   │  ├── SIEM with real-time alerting                                  │   │
    │   │  ├── 24/7 security operations center (SOC)                         │   │
    │   │  └── Threat hunting and intelligence                               │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                    ▲                                       │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LAYER 3: DATA PROTECTION                                           │   │
    │   │  ├── AES-256 encryption at rest                                    │   │
    │   │  ├── TLS encryption in transit                                     │   │
    │   │  └── Hardware security modules (HSMs)                              │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                    ▲                                       │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LAYER 2: NETWORK & APPLICATION SECURITY                            │   │
    │   │  ├── Air-gapped backup systems                                     │   │
    │   │  ├── DDoS protection (multi-terabit capacity)                      │   │
    │   │  ├── Regular penetration testing                                   │   │
    │   │  └── Secure software development lifecycle                         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                    ▲                                       │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  LAYER 1: IDENTITY MANAGEMENT                                       │   │
    │   │  └── Multi-factor authentication for all privileged access         │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    │                                                                             │
    │   RECOVERY OBJECTIVES:                                                     │
    │                                                                             │
    │   RTO (Recovery Time Objective):     < 2 hours for critical systems       │
    │   RPO (Recovery Point Objective):    < 5 minutes data loss                │
    │   Geographic redundancy:             Minimum 2 data centers > 50 km apart │
    │   Annual testing:                    Full failover drills (2x per year)   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Central Bank Communications

### Forward Guidance and Market Impact

```
FORWARD GUIDANCE TYPES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   1. CALENDAR-BASED                                                        │
    │                                                                             │
    │      "Policy rate will remain at current level until Q2 2026"             │
    │                                                                             │
    │      └── Provides certainty about time horizon                            │
    │                                                                             │
    │                                                                             │
    │   2. STATE-BASED (OUTCOME)                                                 │
    │                                                                             │
    │      "Rates will not increase until inflation sustainably reaches 2%"     │
    │                                                                             │
    │      └── Conditions guidance on observable economic outcomes              │
    │                                                                             │
    │                                                                             │
    │   3. STATE-BASED (THRESHOLD)                                               │
    │                                                                             │
    │      "Asset purchases will continue until unemployment falls below 6.5%"  │
    │                                                                             │
    │      └── Clear numerical threshold, easy to communicate                   │
    │                                                                             │
    │                                                                             │
    │   4. OPEN-ENDED                                                            │
    │                                                                             │
    │      "Policy will remain accommodative for an extended period"            │
    │                                                                             │
    │      └── Maximum flexibility, least precise                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    COMMUNICATION CHANNELS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CHANNEL                          FREQUENCY              AUDIENCE         │
    │   ───────────────────────────────────────────────────────────────────────── │
    │   Monetary Policy Statement        6-8 times per year    Public, markets  │
    │   ───────────────────────────────────────────────────────────────────────── │
    │   Press Conference                 After each meeting    Media, public    │
    │   ───────────────────────────────────────────────────────────────────────── │
    │   Meeting Minutes                  3 weeks after         Markets, analysts│
    │   ───────────────────────────────────────────────────────────────────────── │
    │   Quarterly Report                 4 times per year      Public           │
    │   ───────────────────────────────────────────────────────────────────────── │
    │   Speeches by officials            Ongoing (monthly)     Markets, experts │
    │   ───────────────────────────────────────────────────────────────────────── │
    │   Economic Projections             4 times per year      Markets          │
    │   (dot plots)                                                            │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    DOT PLOT EXAMPLE (Federal Reserve)

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Projected Federal Funds Rate (%)                                         │
    │                                                                             │
    │   6.0 ┼                                                                   │
    │       │                                                                   │
    │   5.5 ┼    ● ● ● ● ●                                                      │
    │       │    ● ● ● ● ●                                                      │
    │   5.0 ┼    ● ● ● ● ●   ●                                                  │
    │       │    ● ● ● ● ●   ● ● ● ● ●                                          │
    │   4.5 ┼    ● ● ● ● ●   ● ● ● ● ●   ●                                      │
    │       │                ● ● ● ● ●   ● ● ● ● ●                              │
    │   4.0 ┼                            ● ● ● ● ●   ●                          │
    │       │                                        ● ● ● ● ●                  │
    │   3.5 ┼                                                    ● ● ● ● ●      │
    │       │                                                                ●   │
    │   3.0 ┼                                                                    │
    │       │                                                                    │
    │       └────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬────►          │
    │           2024 2025 2026 2027  Long                                        │
    │                                                                             │
    │   Each dot represents one FOMC participant's rate projection              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
FORMULA REFERENCE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Money Multiplier = 1 / Reserve Requirement Ratio                         │
    │                                                                             │
    │   Required Reserves = RR Ratio × Transaction Deposits                      │
    │                                                                             │
    │   Excess Reserves = Actual Reserves - Required Reserves                    │
    │                                                                             │
    │   Policy Rate Corridor = Lending Rate - Deposit Rate                       │
    │                                                                             │
    │   Real Interest Rate = Nominal Rate - Inflation Rate                       │
    │                                                                             │
    │   Quantity Theory: MV = PQ                                                 │
    │                                                                             │
    │   Taylor Rule: i = r* + π + 0.5(π - π*) + 0.5(y - y*)                     │
    │                                                                             │
    │   Reserve Balance = Assets - Currency - Other Liabilities                  │
    │                                                                             │
    │   Discount Window Penalty (Primary) = Policy Rate + 0.50%                  │
    │                                                                             │
    │   Discount Window Penalty (Secondary) = Policy Rate + 1.00%                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
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