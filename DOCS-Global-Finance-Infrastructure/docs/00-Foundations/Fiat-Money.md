# 04 - Fiat Money

## Documentation Overview

Fiat money is a government-issued currency that is not backed by a physical commodity such as gold or silver. Its value derives from the trust and confidence that people place in the issuing government and the legal tender laws that require its acceptance for payment of debts. This document covers the nature, mechanisms, advantages, risks, and operational processes of fiat money systems.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the definition and nature of fiat money                       │
    │   Learn the distinction between commodity money and fiat money             │
    │   Study the trust-based value mechanism                                    │
    │   Analyze the role of legal tender laws                                     │
    │   Examine the money creation process through banking                       │
    │   Understand seigniorage and its economic implications                     │
    │   Learn central bank roles in fiat systems                                 │
    │   Study inflation risks and hyperinflation failures                        │
    │   Compare fiat to commodity and cryptocurrency alternatives                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Definition and Core Concepts

### What is Fiat Money

Fiat money is currency that a government has declared to be legal tender but is not convertible into a fixed amount of any commodity. The word "fiat" comes from Latin meaning "let it be done" or "by decree." The currency has value because the government mandates its acceptance and because people trust that others will accept it.

```
FIAT MONEY VALUE SOURCES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │                    SOURCES OF FIAT MONEY VALUE                              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                                                                     │   │
    │   │   GOVERNMENT DECREE (Legal Tender)                                  │   │
    │   │   ├── Laws requiring acceptance for debt payment                    │   │
    │   │   ├── Tax payments must be made in the currency                     │   │
    │   │   └── Government salaries and payments made in the currency         │   │
    │   │                                                                     │   │
    │   │   SOCIAL TRUST AND CONVENTION                                       │   │
    │   │   ├── Everyone believes others will accept it                       │   │
    │   │   ├── Past experience of acceptance                                 │   │
    │   │   └── Network effects (more users increase value)                   │   │
    │   │                                                                     │   │
    │   │   SCARCITY (Managed by Central Bank)                                │   │
    │   │   ├── Limited supply controlled by monetary policy                  │   │
    │   │   ├── No unlimited printing without consequences                    │   │
    │   │   └── Credibility of supply constraints                             │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Commodity Money vs Fiat Money

```
COMMODITY VS FIAT MONEY COMPARISON

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Feature              │ Commodity Money        │ Fiat Money               │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Intrinsic value      │ Has value outside      │ No intrinsic value       │
    │                        │ money use (gold,       │ (paper or digital)       │
    │                        │ silver, salt, cattle)  │                          │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Value source         │ Physical properties    │ Government decree +      │
    │                        │ + scarcity             │ social trust             │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Supply flexibility   │ Limited by mining/     │ Potentially unlimited    │
    │                        │ production capacity    │ (but constrained by      │
    │                        │                        │ policy)                  │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Storage cost         │ High (physical         │ Low (digital or paper)   │
    │                        │ security, insurance)   │                          │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Divisibility         │ Limited (physical      │ Highly divisible         │
    │                        │ constraints)           │ (digital to any amount)  │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Portability          │ Poor (heavy,           │ Excellent (light,        │
    │                        │ bulky)                 │ digital transfer)        │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Monetary policy      │ Impossible (supply     │ Full central bank        │
    │   control              │ fixed by mining)       │ control                  │
    │   ─────────────────────│────────────────────────│──────────────────────────│
    │   Examples             │ Gold standard, silver  │ US Dollar, Euro, Yen,    │
    │                        │ standard, gold coins   │ Pound, all modern        │
    │                        │                        │ currencies                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## How Fiat Money Works

### Full Process of Fiat Money Creation and Circulation

```
COMPLETE FIAT MONEY PROCESS FLOW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   STEP 1: MONEY CREATION (Central Bank)                                    │
    │                                                                             │
    │   Central bank creates money by expanding its balance sheet.              │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  CENTRAL BANK BALANCE SHEET EXPANSION                               │   │
    │   │                                                                     │   │
    │   │  ASSETS                    LIABILITIES                              │   │
    │   │  ┌─────────────────────┐   ┌─────────────────────────────────────┐ │   │
    │   │  │ Government Bonds    │   │ Bank Reserves (Newly Created Money) │ │   │
    │   │  │ (+$1 million)       │   │ (+$1 million)                       │ │   │
    │   │  └─────────────────────┘   └─────────────────────────────────────┘ │   │
    │   │                                                                     │   │
    │   │  Two methods:                                                       │   │
    │   │  ├── Open Market Purchase: Buying bonds from banks                 │   │
    │   │  ├── Direct Monetization: Buying bonds from government directly    │   │
    │   │  └── Printing physical currency                                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 2: MONEY ENTERS BANKING SYSTEM                                     │
    │                                                                             │
    │   New reserves credited to commercial bank accounts at central bank.      │
    │                                                                             │
    │   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐                 │
    │   │  Bank A     │     │  Bank B     │     │  Bank C     │                 │
    │   │  Reserves   │     │  Reserves   │     │  Reserves   │                 │
    │   │  +$300k     │     │  +$300k     │     │  +$400k     │                 │
    │   └─────────────┘     └─────────────┘     └─────────────┘                 │
    │        │                   │                   │                           │
    │        └───────────────────┼───────────────────┘                           │
    │                            │                                               │
    │                            ▼                                               │
    │   STEP 3: MULTIPLE DEPOSIT CREATION (Fractional Reserve Banking)          │
    │                                                                             │
    │   Banks lend out excess reserves, creating new deposits.                  │
    │                                                                             │
    │   Initial Reserve Injection: $1,000,000                                   │
    │   Reserve Requirement: 10%                                                │
    │   Money Multiplier: 10                                                    │
    │   Total Money Created: $10,000,000                                        │
    │                                                                             │
    │   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐                   │
    │   │  Bank A     │───►│  Bank B     │───►│  Bank C     │                   │
    │   │  Receives   │    │  Receives   │    │  Receives   │                   │
    │   │  $1M        │    │  $900k      │    │  $810k      │                   │
    │   │  Lends $900k│    │  Lends $810k│    │  Lends $729k│                   │
    │   └─────────────┘    └─────────────┘    └─────────────┘                   │
    │        │                   │                   │                           │
    │        └───────────────────┼───────────────────┘                           │
    │                            │                                               │
    │                            ▼                                               │
    │   STEP 4: MONEY CIRCULATES IN ECONOMY                                     │
    │                                                                             │
    │   Money used for transactions, wages, purchases, investments.             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │                         ECONOMY                                     │   │
    │   │                                                                     │   │
    │   │   ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐         │   │
    │   │   │ Wages   │───►│ Rent    │───►│ Goods   │───►│ Savings │         │   │
    │   │   │ $500    │    │ $200    │    │ $300    │    │ $100    │         │   │
    │   │   └─────────┘    └─────────┘    └─────────┘    └─────────┘         │   │
    │   │                                                                     │   │
    │   │   Transactions occur at market prices determined by supply/demand   │   │
    │   │                                                                     │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   STEP 5: TAXATION AND MONEY DESTRUCTION                                  │
    │                                                                             │
    │   Government collects taxes, removing money from circulation.             │
    │                                                                             │
    │   ┌─────────────────────────────────────────────────────────────────────┐   │
    │   │  Tax Payment → Government → Central Bank (Money Destroyed)          │   │
    │   │                                                                     │   │
    │   │  Alternative: Government spends money back into economy             │   │
    │   │  (fiscal policy)                                                    │   │
    │   └─────────────────────────────────────────────────────────────────────┘   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Legal Tender Mechanism

Legal Tender Definition: Legal tender laws require that the designated currency must be accepted for payment of debts, taxes, and other monetary obligations within the issuing jurisdiction.

How it works: A debtor cannot successfully sue for non-payment if they offered to pay in legal tender and the creditor refused. By mandating acceptance for debt payments, the government creates a guaranteed use case for the currency. All taxes must be paid in the currency, creating a constant demand. Government pays its employees, contractors, and benefit recipients in the currency, further circulating it.

```
LEGAL TENDER HIERARCHY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   GOVERNMENT DECLARES FIAT CURRENCY AS LEGAL TENDER                        │
    │        │                                                                   │
    │        ▼                                                                   │
    │   TAXES MUST BE PAID IN THAT CURRENCY                                      │
    │        │                                                                   │
    │        ▼                                                                   │
    │   CITIZENS NEED CURRENCY FOR TAX PAYMENT                                   │
    │        │                                                                   │
    │        ▼                                                                   │
    │   EMPLOYERS PAY WAGES IN THAT CURRENCY                                     │
    │        │                                                                   │
    │        ▼                                                                   │
    │   WORKERS ACCEPT CURRENCY FOR LABOR                                         │
    │        │                                                                   │
    │        ▼                                                                   │
    │   SHOPS ACCEPT CURRENCY TO PAY WORKERS AND TAXES                           │
    │        │                                                                   │
    │        ▼                                                                   │
    │   ACCEPTANCE BECOMES UNIVERSAL (Self-reinforcing cycle)                    │
    │        │                                                                   │
    │        ▼                                                                   │
    │   FIAT MONEY FUNCTIONS AS MEDIUM OF EXCHANGE                               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Functions of Money in Fiat System

```
FUNCTIONS OF MONEY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FUNCTION          │ HOW FIAT PERFORMS           │ IMPORTANCE             │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Medium of         │ Accepted universally for   │ Eliminates barter      │
    │   exchange          │ transactions by law and    │ double coincidence     │
    │                     │ convention                 │ of wants problem       │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Unit of account   │ Prices denominated in      │ Enables economic       │
    │                     │ fiat units ($, €, ¥)        │ calculation and        │
    │                     │                            │ comparison             │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Store of value    │ Holds value over time      │ Enables saving and     │
    │                     │ (subject to inflation      │ deferred payment       │
    │                     │ risk)                      │                        │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Standard of       │ Used for future payments   │ Enables lending,       │
    │   deferred payment  │ (loans, bonds, contracts)  │ credit, and debt       │
    │                     │ denominated in fiat        │ markets                │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Seigniorage

### Definition and Mechanism

Seigniorage is the profit earned by the government or central bank from issuing currency. It represents the difference between the face value of money and the cost of producing and distributing it.

How it works: For physical currency, a $100 bill costs approximately $0.14 to print. The $99.86 difference is seigniorage profit for the government. For digital money (bank reserves), the cost of creation is effectively zero. Any newly created money that enters circulation represents seigniorage revenue.

```
SEIGNIORAGE CALCULATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   PHYSICAL CURRENCY:                                                       │
    │                                                                             │
    │   Seigniorage = Face Value - Production Cost                               │
    │                                                                             │
    │   Example ($100 bill):                                                     │
    │   Face Value: $100.00                                                      │
    │   Production Cost: $0.14                                                   │
    │   Seigniorage: $99.86 per bill                                             │
    │                                                                             │
    │                                                                             │
    │   DIGITAL CURRENCY (Reserves):                                             │
    │                                                                             │
    │   Seigniorage = Face Value - Zero Production Cost                          │
    │                                                                             │
    │   Example ($1 million digital creation):                                   │
    │   Seigniorage: $1 million                                                  │
    │                                                                             │
    │                                                                             │
    │   ANNUAL SEIGNIORAGE REVENUE (Selected countries):                         │
    │                                                                             │
    │   United States: ~$70 billion per year                                     │
    │   Eurozone: ~€50 billion per year                                          │
    │   Japan: ~¥2 trillion per year                                             │
    │   United Kingdom: ~£10 billion per year                                    │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### How Seigniorage Benefits Government

Seigniorage reduces the need for other taxes. When the government spends newly created money, it acquires real resources (goods, services, labor) without having to collect taxes first. This is sometimes called "monetizing spending" or "printing money to pay bills."

How it works: The central bank creates money to purchase government bonds (or directly funds government spending). The government uses this money to pay its obligations. The new money enters circulation. The government effectively received resources without taxing citizens. The cost to citizens is the potential inflation from increased money supply.

## Central Bank Operations in Fiat System

### Monetary Policy Tools in Fiat Money

Fiat money gives central banks the ability to actively manage money supply and interest rates to pursue economic goals such as price stability, full employment, and financial stability.

```
CENTRAL BANK POLICY TOOLS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TOOL              │ HOW IT WORKS                │ EFFECT ON MONEY        │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Policy Rate       │ Interest rate on bank      │ Higher rate reduces     │
    │   (Interest on      │ reserves at central bank   │ lending and money       │
    │   Reserves)         │                            │ creation. Lower rate    │
    │                     │                            │ increases.              │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Open Market       │ Central bank buys or sells │ Purchase injects        │
    │   Operations        │ government bonds           │ money. Sale removes     │
    │                     │                            │ money.                  │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Reserve           │ Required reserves as % of  │ Higher requirement      │
    │   Requirements      │ deposits                   │ reduces money           │
    │                     │                            │ multiplier. Lower       │
    │                     │                            │ increases.              │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Quantitative      │ Large-scale asset          │ Injects large amounts   │
    │   Easing            │ purchases beyond normal    │ directly into           │
    │                     │ OMO                        │ financial system        │
    │   ──────────────────│────────────────────────────│────────────────────────│
    │   Forward Guidance  │ Communication of future    │ Shapes expectations,    │
    │                     │ policy path                │ influences long-term    │
    │                     │                            │ rates                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Money Supply Measurement

```
MONEY SUPPLY AGGREGATES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   AGGREGATE      │ COMPONENTS                      │ LIQUIDITY             │
    │   ───────────────│─────────────────────────────────│───────────────────────│
    │   M0 (Monetary   │ Physical currency (coins,       │ Most liquid           │
    │   Base)          │ banknotes) + Bank reserves      │                       │
    │                  │ at central bank                 │                       │
    │   ───────────────│─────────────────────────────────│───────────────────────│
    │   M1             │ M0 + Demand deposits +          │ Very liquid           │
    │                  │ Traveler's checks + Other       │                       │
    │                  │ checkable deposits              │                       │
    │   ───────────────│─────────────────────────────────│───────────────────────│
    │   M2             │ M1 + Savings deposits +         │ Moderately liquid     │
    │                  │ Small time deposits +           │                       │
    │                  │ Money market mutual funds       │                       │
    │   ───────────────│─────────────────────────────────│───────────────────────│
    │   M3 (Less       │ M2 + Large time deposits +      │ Less liquid           │
    │   common)        │ Institutional money funds +     │                       │
    │                  │ Repurchase agreements           │                       │
    │                                                                             │
    │                                                                             │
    │   MONEY MULTIPLIER (Reserve Ratio = 10%)                                    │
    │                                                                             │
    │   Money Multiplier = 1 / Reserve Ratio = 1 / 0.10 = 10                     │
    │                                                                             │
    │   Total Money Supply (M1) = Monetary Base × Money Multiplier               │
    │                                                                             │
    │   If Monetary Base = $1 trillion:                                          │
    │   M1 = $1 trillion × 10 = $10 trillion                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Inflation in Fiat Money Systems

### Why Fiat Money Loses Value

Inflation occurs when the money supply grows faster than the supply of goods and services. Fiat money has no intrinsic value and no fixed supply, so over-issuance is possible.

```
INFLATION MECHANISM

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   EXCESSIVE MONEY CREATION                                                 │
    │        │                                                                   │
    │        ▼                                                                   │
    │   MORE MONEY CHASING SAME AMOUNT OF GOODS                                  │
    │        │                                                                   │
    │        ▼                                                                   │
    │   PRICES RISE                                                              │
    │        │                                                                   │
    │        ▼                                                                   │
    │   PURCHASING POWER OF EACH MONETARY UNIT FALLS                            │
    │        │                                                                   │
    │        ├─────────────────────────────────────────────────────┐            │
    │        ▼                                                     ▼            │
    │   SAVERS LOSE VALUE                                     DEBTORS BENEFIT   │
    │   (Real returns negative)                               (Repay with        │
    │                                                        cheaper money)      │
    │                                                                             │
    │                                                                             │
    │   QUANTITY THEORY OF MONEY: MV = PQ                                        │
    │                                                                             │
    │   M = Money Supply                                                         │
    │   V = Velocity of Money (assumed constant)                                 │
    │   P = Price Level                                                          │
    │   Q = Real Output                                                          │
    │                                                                             │
    │   If M increases faster than Q, P must rise (inflation)                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Hyperinflation

Hyperinflation occurs when inflation becomes extremely rapid and out of control, often exceeding 50% per month. Fiat money systems can fail completely when trust collapses.

Causes: Government prints money to cover massive budget deficits. Loss of confidence leads to rapid spending (velocity increases). Prices spiral upward. Money becomes worthless.

How it works: Government cannot tax or borrow enough to cover spending. Central bank directly finances government (monetizing debt). Money supply explodes. People lose faith and spend money immediately upon receipt. Prices rise faster than money creation. The cycle accelerates until currency becomes worthless.

```
HYPERINFLATION EXAMPLES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Country        │ Period          │ Peak Monthly   │ Price Increase       │
    │                  │                 │ Inflation      │ (over period)        │
    │   ───────────────│─────────────────│────────────────│──────────────────────│
    │   Weimar Germany │ 1921-1923       │ 29,500%        │ 1,000,000,000:1      │
    │   (1923)         │                 │ (Oct 1923)     │ (over 2 years)        │
    │   ───────────────│─────────────────│────────────────│──────────────────────│
    │   Zimbabwe       │ 2007-2009       │ 79,600,000,000%│ 10,000,000,000,000:1  │
    │                  │                 │ (Nov 2008)     │                       │
    │   ───────────────│─────────────────│────────────────│──────────────────────│
    │   Yugoslavia     │ 1992-1994       │ 313,000,000%   │ 100,000,000,000:1     │
    │   ───────────────│─────────────────│────────────────│──────────────────────│
    │   Hungary        │ 1945-1946       │ 41,900,000,000,│ 400,000,000,000,000, │
    │                  │                 │ 000% (July 46) │ 000,000,000,000,000:1 │
    │   ───────────────│─────────────────│────────────────│──────────────────────│
    │   Venezuela      │ 2016-2021       │ 53,000,000%    │ 100,000,000:1        │
    │                  │                 │ (2019)         │                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Advantages of Fiat Money

### Flexibility for Monetary Policy

Central banks can respond to economic conditions by adjusting money supply. During recessions, money supply can be increased to stimulate demand. During booms, money supply can be reduced to prevent overheating.

How it works: Unlike gold standard where money supply is tied to gold discoveries, fiat money supply can be actively managed. The central bank can inject liquidity during financial crises (2008, 2020). It can lower interest rates to encourage borrowing during recessions. It can raise rates to fight inflation.

### Low Production and Transaction Costs

Fiat money is inexpensive to produce compared to commodity money. Digital fiat costs almost nothing to create and transfer.

How it works: Physical currency costs pennies per note regardless of denomination. Electronic transfers cost fractions of a cent per transaction. A gold coin would require mining, refining, minting, and secure storage. Fiat eliminates these costs.

### Elastic Supply

Money supply can expand or contract with economic needs. A growing economy needs more money to facilitate transactions without deflation.

How it works: As population and output grow, fiat money supply can increase accordingly. Under gold standard, money supply grows only as fast as gold mining. This could cause deflation during periods of rapid economic growth. Fiat avoids this constraint.

### Seigniorage Revenue

Government earns profit from money creation, reducing need for other taxes.

How it works: Every dollar created and circulated represents revenue to the government. The US Treasury earned approximately $70 billion in seigniorage in 2023. This is essentially a tax on cash holders (inflation tax) but is typically modest in stable economies.

## Disadvantages and Risks of Fiat Money

### Inflation Risk

The primary risk of fiat money is inflation, which erodes purchasing power and savings.

How it works: If central bank creates money faster than economic growth, inflation results. Savers see real value of their savings decline. Fixed-income earners (pensioners, bondholders) are harmed. Uncertainty about future inflation distorts economic decisions.

### Hyperinflation Risk

Under extreme conditions, fiat money can become worthless through hyperinflation.

How it works: When government loses fiscal discipline and relies on central bank financing, money supply explodes. Public loses confidence and velocity increases dramatically. Hyperinflation becomes self-reinforcing. Currency may be abandoned for foreign currency, gold, or barter.

### Trust Dependence

Fiat money has no intrinsic value and depends entirely on trust in the issuing government.

How it works: If trust collapses (political instability, government default, regime change), the currency can become worthless overnight. Unlike gold which retains value regardless of government, fiat has no fallback. This trust must be continuously maintained.

### Political Pressure for Monetization

Governments may pressure central banks to print money to finance spending rather than raise taxes.

How it works: Printing money is politically easier than raising taxes or cutting spending. The cost (inflation) is dispersed across all currency holders rather than directly visible to voters. This creates chronic inflation bias in some countries.

## Fiat Money vs Alternatives

### Fiat vs Gold Standard

```
FIAT VS GOLD STANDARD

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Aspect            │ Fiat Money              │ Gold Standard              │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Supply control    │ Active (central bank)   │ Passive (mining rate)      │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Inflation         │ Possible (policy error) │ Low (limited supply)       │
    │   response          │                         │                            │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Deflation         │ Possible (policy error) │ Common (supply fixed,      │
    │   response          │                         │ output grows)              │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Crisis response   │ Can inject liquidity   │ Constrained (limited gold)  │
    │   (2008, 2020)      │ freely                 │                            │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Seigniorage       │ Full profit to         │ None (gold miners profit)   │
    │                     │ government              │                            │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   International     │ Floating exchange      │ Fixed exchange rates       │
    │   adjustment        │ rates                   │ (often unstable)           │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Current system    │ Universal since 1971   │ Ended 1914-1971            │
    │                     │ (Nixon shock)           │ (final US gold window      │
    │                     │                         │ closed 1971)               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

### Fiat vs Cryptocurrency

```
FIAT VS CRYPTOCURRENCY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Aspect            │ Fiat Money              │ Cryptocurrency (Bitcoin)   │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Issuer            │ Government / Central    │ No central issuer          │
    │                     │ Bank                    │ (algorithmic)              │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Supply limit      │ No fixed limit          │ Fixed (21 million BTC)     │
    │                     │ (policy constrained)    │                            │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Transaction cost  │ Low (especially         │ High (energy, fees)        │
    │                     │ digital)                │                            │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Transaction speed │ Very fast (digital)     │ Slow (10-60 minutes)       │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Legal tender      │ Yes (by law)            │ No (in most countries)     │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Backing           │ Government decree +     │ Cryptographic proof +      │
    │                     │ trust                   │ consensus                  │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Price volatility  │ Low (stable economies)  │ Very high (>50% annual)    │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Monetary policy   │ Active management       │ None (fixed supply)        │
    │   ──────────────────│────────────────────────│────────────────────────────│
    │   Adoption          │ Universal               │ Niche (few transactions)   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## The Full Fiat Money Lifecycle

```
COMPLETE LIFECYCLE OF FIAT MONEY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CREATION                                                                 │
    │   │                                                                        │
    │   ├── Central bank creates reserves (digital)                             │
    │   ├── Treasury mints coins and prints notes (physical)                    │
    │   └── Commercial banks create deposits through lending                    │
    │   │                                                                        │
    │   ▼                                                                        │
    │   CIRCULATION                                                             │
    │   │                                                                        │
    │   ├── Wages paid to workers                                              │
    │   ├── Consumers buy goods and services                                    │
    │   ├── Businesses pay suppliers and taxes                                  │
    │   ├── Banks lend to borrowers                                             │
    │   └── Government spends on programs                                       │
    │   │                                                                        │
    │   ▼                                                                        │
    │   VALUE CHANGE (Inflation or Deflation)                                   │
    │   │                                                                        │
    │   ├── If money supply grows faster than output → Inflation               │
    │   ├── If money supply grows slower than output → Deflation               │
    │   └── Purchasing power changes over time                                 │
    │   │                                                                        │
    │   ▼                                                                        │
    │   DESTRUCTION                                                             │
    │   │                                                                        │
    │   ├── Taxes paid to government (removed from circulation)                │
    │   ├── Central bank sells bonds (absorbs reserves)                        │
    │   ├── Physical currency withdrawn and destroyed (worn out)               │
    │   └── Loans repaid (deposits destroyed in fractional reserve)            │
    │   │                                                                        │
    │   ▼                                                                        │
    │   SYSTEM FAILURE (Potential)                                              │
    │   │                                                                        │
    │   ├── Hyperinflation: Currency becomes worthless                         │
    │   ├── Currency abandonment: Shift to foreign currency                    │
    │   ├── Monetary reform: New currency issued (redenomination)              │
    │   └── Return to commodity backing or cryptocurrency                      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Formulas Quick Reference

```
FIAT MONEY FORMULAS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Quantity Theory: MV = PQ                                                 │
    │   M = Money Supply                                                         │
    │   V = Velocity of Money                                                    │
    │   P = Price Level                                                          │
    │   Q = Real Output                                                          │
    │                                                                             │
    │   Money Multiplier = 1 / Reserve Requirement Ratio                         │
    │                                                                             │
    │   Total Money Supply = Monetary Base × Money Multiplier                    │
    │                                                                             │
    │   Seigniorage (Physical) = Face Value - Production Cost                    │
    │                                                                             │
    │   Seigniorage (Digital) = Face Value (effective)                           │
    │                                                                             │
    │   Inflation Rate = (CPI_current - CPI_previous) / CPI_previous × 100      │
    │                                                                             │
    │   Real Value of Money = Nominal Value / Price Level                        │
    │                                                                             │
    │   Real Interest Rate = Nominal Rate - Inflation Rate                       │
    │                                                                             │
    │   Purchasing Power Decline = 1 - (1 / (1 + Inflation Rate))                │
    │   Example: 10% inflation → 1 - (1/1.1) = 9.1% decline in purchasing power  │
    │                                                                             │
    │   Hyperinflation (Cagan model): ln(P) = ln(M) × α + constant              │
    │   (Prices increase exponentially with money supply during hyperinflation)  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## Summary

1. Fiat money is government-issued currency not backed by any commodity. Value derives from trust, legal tender laws, and managed scarcity.

2. Commodity money has intrinsic value (gold, silver). Fiat has no intrinsic value but is more flexible and cheaper to produce.

3. Money creation process: Central bank creates reserves → banks lend → money multiplier expands supply → money circulates.

4. Legal tender laws require acceptance for debts and taxes, creating guaranteed demand and universal acceptance.

5. Seigniorage is government profit from issuing money. US earns ~$70 billion annually. Digital creation cost is near zero.

6. Functions of money: Medium of exchange, unit of account, store of value, standard of deferred payment.

7. Central bank tools: Policy rate, open market operations, reserve requirements, quantitative easing, forward guidance.

8. Money supply aggregates: M0 (monetary base), M1 (narrow money), M2 (broad money). Multiplier determines total supply.

9. Inflation occurs when money supply grows faster than output. Quantity theory: MV = PQ.

10. Hyperinflation results from extreme money creation and loss of trust. Examples: Weimar Germany, Zimbabwe, Hungary.

11. Advantages: Monetary policy flexibility, low production costs, elastic supply, seigniorage revenue.

12. Disadvantages: Inflation risk, hyperinflation risk, trust dependence, political pressure for monetization.

13. Fiat vs Gold Standard: Fiat allows active policy but inflation possible. Gold prevents inflation but causes deflation and limits crisis response.

14. Fiat vs Cryptocurrency: Fiat is legal tender, low volatility, government-backed. Crypto is decentralized, fixed supply, high volatility.

15. Full lifecycle: Creation (central bank/commercial banks) → Circulation (economy) → Value change (inflation/deflation) → Destruction (taxes/bond sales) → Potential system failure.

16. Fiat money works because everyone believes it works. This self-referential trust is both its strength and its vulnerability.

*This documentation belongs to https://github.com/InterCentury*