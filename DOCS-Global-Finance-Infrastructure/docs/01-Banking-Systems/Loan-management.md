# Loan-management

## Documentation Overview

Loans are the primary mechanism through which banks create money and drive economic activity. When a bank makes a loan, it does not lend existing deposits—it creates new money. This document explains the complete lifecycle of loans, from application to repayment, and the critical role loans play in money creation, fractional reserve banking, and economic growth.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   Understand what a loan is and its fundamental purpose                     │
    │   Learn why individuals and businesses borrow money                         │
    │   Study the different types of loans and their characteristics              │
    │   Examine the loan application and approval process                         │
    │   Understand interest calculation and repayment mechanisms                  │
    │   Learn how banks create money through lending                              │
    │   Study fractional reserve banking and its limitations                      │
    │   Analyze the relationship between lending, inflation, and growth           │
    │   Understand loan default, NPLs, and risk management                        │
    │   Learn the complete lifecycle of a bank loan                               │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 1. What is a Loan

A loan is a financial transaction in which one party (the lender) provides money or assets to another party (the borrower) with the expectation of repayment, usually with interest, at a future date. Loans are a form of debt and create a legal obligation for the borrower to repay the principal amount plus any agreed-upon interest.

How it works: The lender provides a lump sum of money to the borrower. The borrower uses the funds for a specific purpose—purchasing a home, financing a business, or covering expenses. The borrower agrees to repay the money over a set period through regular payments that include both principal and interest. The lender earns a return (interest) for the use of their money and for taking on the risk that the borrower might default.

```
BASIC LOAN STRUCTURE

                         +---------------------------+
                         |        LENDER             |
                         |        (Bank)             |
                         +-------------+-------------+
                                       |
                                       | Provides Principal
                                       | (Lump sum)
                                       ▼
                         +---------------------------+
                         |        BORROWER           |
                         |   (Individual/Business)   |
                         +-------------+-------------+
                                       |
                                       | Repays Principal + Interest
                                       | (Regular payments over time)
                                       ▼
                         +---------------------------+
                         |         LENDER            |
                         |         (Bank)            |
                         +---------------------------+

    KEY COMPONENTS:
    +---------------------------+
    |  Principal: Original amount borrowed
    |  Interest: Cost of borrowing (fee for using money)
    |  Term: Time period for repayment
    |  Payment Schedule: Regular installments
    |  Collateral: Assets pledged as security (if secured)
    |  Legal Agreement: Contract specifying terms
    +---------------------------+
```

## 2. Why Do People and Businesses Take Loans

People and businesses borrow money for various reasons, all centered around the need for funds that exceed current available resources.

How it works: Borrowing allows individuals and businesses to make purchases or investments that they could not afford with their current savings. The borrower pays a cost (interest) for the privilege of accessing funds today. The lender earns a return on their capital. This exchange enables economic activity that would otherwise not occur.

```
WHY PEOPLE BORROW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   REASON 1: BIG TICKET PURCHASES                                            │
    │   ├── Home purchase (mortgage)                                              │
    │   ├── Vehicle purchase (auto loan)                                          │
    │   └── Education (student loan)                                              │
    │                                                                             │
    │   REASON 2: BRIDGING CASH FLOW GAPS                                         │
    │   ├── Unexpected emergencies (medical, repairs)                             │
    │   ├── Temporary income shortfall                                            │
    │   └── Seasonal business needs                                               │
    │                                                                             │
    │   REASON 3: CONSOLIDATING DEBT                                              │
    │   ├── Combining multiple debts into one loan                                │
    │   ├── Lowering overall interest cost                                        │
    │   └── Simplifying monthly payments                                          │
    │                                                                             │
    │   REASON 4: BUILDING CREDIT HISTORY                                         │
    │   ├── Establishing a credit record                                          │
    │   ├── Demonstrating responsible borrowing                                   │
    │   └── Qualifying for future, larger loans                                   │
    └─────────────────────────────────────────────────────────────────────────────┘

WHY BUSINESSES BORROW

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   REASON 1: CAPITAL EXPENDITURE (CAPEX)                                     │
    │   ├── Purchasing equipment and machinery                                    │
    │   ├── Buying real estate for operations                                     │
    │   └── Technology upgrades and infrastructure                                │
    │                                                                             │
    │   REASON 2: WORKING CAPITAL                                                 │
    │   ├── Funding inventory purchases                                           │
    │   ├── Covering payroll during slow seasons                                  │
    │   └── Managing accounts receivable gaps                                     │
    │                                                                             │
    │   REASON 3: EXPANSION AND GROWTH                                            │
    │   ├── Opening new locations                                                 │
    │   ├── Entering new markets                                                  │
    │   └── Acquiring competitors                                                 │
    │                                                                             │
    │   REASON 4: RESEARCH AND DEVELOPMENT                                        │
    │   ├── Developing new products                                               │
    │   ├── Patent and innovation investment                                      │
    │   └── Hiring specialized talent                                             │
    │                                                                             │
    │   REASON 5: LEVERAGE                                                        │
    │   ├── Using borrowed money to amplify returns                               │
    │   ├── Maintaining ownership instead of issuing equity                       │
    │   └── Taking advantage of interest tax deductions                           │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 3. Who Can Issue Loans

Loans can be issued by various types of financial institutions and entities.

```
LOAN ISSUERS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   ISSUER 1: COMMERCIAL BANKS                                                │
    │   ├── Largest providers of loans                                            │
    │   ├── Offer all types of loans (mortgages, auto, business, personal)        │
    │   ├── Regulated by central banks and banking authorities                    │
    │   └── Create money through lending (fractional reserve)                     │
    │                                                                             │
    │   ISSUER 2: CREDIT UNIONS                                                   │
    │   ├── Member-owned cooperatives                                             │
    │   ├── Typically offer lower rates                                           │
    │   ├── Focus on consumer loans and auto loans                                │
    │   └── Limited to members                                                    │
    │                                                                             │
    │   ISSUER 3: FINANCE COMPANIES                                               │
    │   ├── Specialize in specific loan types                                     │
    │   ├── Auto finance, mortgage companies, payday lenders                      │
    │   ├── Often higher rates than banks                                         │
    │   └── Less regulated than banks                                             │
    │                                                                             │
    │   ISSUER 4: ONLINE LENDERS (FINTECH)                                        │
    │   ├── Digital-first lending platforms                                       │
    │   ├── Faster approval and disbursement                                      │
    │   ├── Use alternative credit scoring models                                 │
    │   └── Peer-to-peer lending platforms                                        │
    │                                                                             │
    │   ISSUER 5: GOVERNMENT AGENCIES                                             │
    │   ├── Student loans (Direct Loans)                                          │
    │   ├── Small Business Administration (SBA) loans                             │
    │   ├── USDA and FHA mortgages                                                │
    │   └── Often subsidized with favorable terms                                 │
    │                                                                             │
    │   ISSUER 6: INSURANCE COMPANIES                                             │
    │   ├── Policy loans (borrowing against life insurance)                       │
    │   ├── Commercial real estate lending                                        │
    │   └── Private placement debt                                                │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 4. What Are the Different Types of Loans

Loans can be categorized by purpose, security, and repayment structure.

```
LOAN TYPES BY PURPOSE

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │   MORTGAGE LOANS                                                            │
    │   ├── Purpose: Purchase or refinance real estate                            │
    │   ├── Term: 15-30 years                                                     │
    │   ├── Secured by property                                                   │
    │   └── Lower interest rates (collateral reduces risk)                        │
    │                                                                             │
    │   AUTO LOANS                                                                │
    │   ├── Purpose: Purchase a vehicle                                           │
    │   ├── Term: 3-7 years                                                       │
    │   ├── Secured by the vehicle                                                │
    │   └── Moderate interest rates                                               │
    │                                                                             │
    │   STUDENT LOANS                                                             │
    │   ├── Purpose: Fund education expenses                                      │
    │   ├── Term: 10-30 years                                                     │
    │   ├── Government or private                                                 │
    │   └── Often deferred payments while studying                                │
    │                                                                             │
    │   PERSONAL LOANS                                                            │
    │   ├── Purpose: General use (debt consolidation, emergencies)                │
    │   ├── Term: 1-7 years                                                       │
    │   ├── Unsecured (no collateral)                                             │
    │   └── Higher interest rates (more risk)                                     │
    │                                                                             │
    │   BUSINESS LOANS                                                            │
    │   ├── Purpose: Business operations, equipment, working capital              │
    │   ├── Term: 1-10 years                                                      │
    │   ├── Secured or unsecured                                                  │
    │   └── Based on business performance                                         │
    │                                                                             │
    │   PAYDAY LOANS                                                              │
    │   ├── Purpose: Short-term cash need until payday                            │
    │   ├── Term: 2-4 weeks                                                       │
    │   ├── Unsecured                                                             │
    │   └── Very high interest rates (predatory)                                  │
    └─────────────────────────────────────────────────────────────────────────────┘

LOAN TYPES BY SECURITY

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   SECURED LOANS                                                            │
    │   │                                                                        │
    │   ├── Backed by collateral (asset)                                        │
    │   ├── Lower interest rates                                                │
    │   ├── Lender can seize asset on default                                  │
    │   └── Examples: Mortgage, auto loan, secured personal loan               │
    │   │                                                                        │
    │   │                                                                        │
    │   UNSECURED LOANS                                                          │
    │   │                                                                        │
    │   ├── No collateral required                                              │
    │   ├── Higher interest rates (more risk)                                  │
    │   ├── Based on credit score and income                                   │
    │   └── Examples: Credit cards, personal loans, student loans              │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 5. How Does the Loan Application Process Work

The loan application process involves several steps from initial inquiry to final approval and disbursement.

How it works: A borrower submits a formal application with personal and financial information. The lender reviews the application, checks credit history, verifies income and assets, and evaluates the borrower's ability to repay. If approved, the lender disburses the funds, and the borrower begins repayment.

```
LOAN APPLICATION PROCESS FLOW

                         +---------------------------+
                         |  STEP 1: APPLICATION      |
                         |  Borrower submits details  |
                         |  - Personal information    |
                         |  - Income/employment       |
                         |  - Loan amount/purpose    |
                         |  - Existing debts         |
                         +-------------+-------------+
                                       |
                                       ▼
                         +---------------------------+
                         |  STEP 2: CREDIT CHECK     |
                         |  - Pull credit report     |
                         |  - Check credit score    |
                         |  - Review payment history |
                         |  - Verify identity       |
                         +-------------+-------------+
                                       |
                                       ▼
                         +---------------------------+
                         |  STEP 3: DOCUMENTATION    |
                         |  - Proof of income       |
                         |  - Bank statements       |
                         |  - Tax returns           |
                         |  - Asset verification    |
                         +-------------+-------------+
                                       |
                                       ▼
                         +---------------------------+
                         |  STEP 4: UNDERWRITING    |
                         |  - Evaluate risk         |
                         |  - Calculate DTI        |
                         |  - Determine eligibility |
                         |  - Set terms/rate       |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  APPROVED         |   |  DECLINED                 |
               |  - Offer made    |   |  - Notified              |
               |  - Terms set    |   |  - Reason provided       |
               |  - Disbursement |   |  - May appeal           |
               +-------------------+   +---------------------------+
                         │
                         ▼
               +---------------------------+
               |  STEP 5: CLOSING          |
               |  - Sign loan agreement    |
               |  - Accept terms           |
               |  - Funds disbursed        |
               +---------------------------+
```

## 6. How Is a Loan Approved

Loan approval is based on the lender's assessment of the borrower's ability and willingness to repay. This is typically evaluated using the "Five C's of Credit."

```
FIVE C'S OF CREDIT

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   1. CHARACTER                                                             │
    │      ├── Borrower's reputation and trustworthiness                         │
    │      ├── Credit history and payment record                                │
    │      ├── FICO/VantageScore score                                          │
    │      └── Past bankruptcies or defaults                                    │
    │                                                                             │
    │   2. CAPACITY                                                              │
    │      ├── Ability to repay                                                 │
    │      ├── Debt-to-income ratio (DTI)                                       │
    │      ├── Income stability                                                 │
    │      └── Employment history                                               │
    │                                                                             │
    │   3. CAPITAL                                                               │
    │      ├── Borrower's net worth                                             │
    │      ├── Down payment or equity contribution                             │
    │      ├── Liquid assets available                                          │
    │      └── Skin in the game                                                │
    │                                                                             │
    │   4. COLLATERAL                                                            │
    │      ├── Assets pledged to secure loan                                   │
    │      ├── Loan-to-value ratio (LTV)                                       │
    │      ├── Quality and liquidity of collateral                              │
    │      └── Appraised value                                                 │
    │                                                                             │
    │   5. CONDITIONS                                                            │
    │      ├── Purpose of loan                                                  │
    │      ├── Economic environment                                             │
    │      ├── Industry conditions                                              │
    │      ├── Interest rate environment                                        │
    │      └── Loan terms and covenants                                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘


    DECISION PROCESS

                         +---------------------------+
                         |    Underwriting Review    |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  All criteria met  |   |  Criteria not met         |
               |  Low risk level    |   |  High risk level          |
               +-------------------+   +---------------------------+
                         │                           │
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  LOAN APPROVED    |   |  LOAN DECLINED            |
               |  - Rate assigned  |   |  - Counter-offer?        |
               |  - Terms set     |   |  - Conditional?          |
               |  - Ready to close |   |  - Alternative product?  |
               +-------------------+   +---------------------------+
```

## 7. What Is Collateral

Collateral is an asset that a borrower pledges to a lender as security for a loan. If the borrower defaults, the lender can seize the collateral to recover the loan amount.

How it works: The lender takes a legal interest (lien) in the collateral. If the borrower fails to repay, the lender can foreclose on or repossess the asset, sell it, and use the proceeds to offset the outstanding debt. Collateral reduces the lender's risk, which typically results in lower interest rates for the borrower.

```
COLLATERAL EXAMPLE (MORTGAGE)

                         +---------------------------+
                         |         BANK              |
                         |       (Lender)            |
                         +-------------+-------------+
                                       |
                                       | Loan of $200,000
                                       | at 5% interest
                                       ▼
                         +---------------------------+
                         |       BORROWER            |
                         |   (Homeowner)             |
                         +-------------+-------------+
                                       |
                                       | Pledges property
                                       | as collateral
                                       ▼
                         +---------------------------+
                         |      PROPERTY             |
                         |    (Collateral)           |
                         |    Value: $250,000        |
                         +---------------------------+

    IF BORROWER DEFAULTS:

                         +---------------------------+
                         |         BANK              |
                         +-------------+-------------+
                                       |
                                       | Forecloses on property
                                       ▼
                         +---------------------------+
                         |      PROPERTY             |
                         |    (Seized by bank)       |
                         +-------------+-------------+
                                       |
                                       | Sold for $220,000
                                       ▼
                         +---------------------------+
                         |  Bank recovers $220,000   |
                         |  Loan balance: $190,000   |
                         |  Bank recovers full debt  |
                         +---------------------------+
```

## 8. What Is an Unsecured Loan

An unsecured loan is a loan that does not require collateral. The lender relies solely on the borrower's creditworthiness and promise to repay.

How it works: The lender approves the loan based on the borrower's income, credit score, and financial history. No specific asset is pledged. If the borrower defaults, the lender must pursue legal action to collect the debt (lawsuit, wage garnishment, or asset seizure through court order). Because the lender has no collateral to seize, unsecured loans carry higher interest rates.

```
SECURED VS UNSECURED LOANS

                         +---------------------------+
                         |     SECURED LOAN          |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  COLLATERAL       |   |  LOWER RISK               |
               |  Asset pledged    |   |  Lower interest rate      |
               |  Can be seized    |   |  Higher approval chance   |
               |  Examples:        |   |  Examples:               |
               |  Mortgage         |   |  Mortgage               |
               |  Auto loan        |   |  Auto loan              |
               +-------------------+   +---------------------------+


                         +---------------------------+
                         |    UNSECURED LOAN          |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  NO COLLATERAL    |   |  HIGHER RISK              |
               |  No asset pledged |   |  Higher interest rate     |
               |  Legal action only|   |  Lower approval chance    |
               |  Examples:        |   |  Examples:               |
               |  Credit cards     |   |  Credit cards            |
               |  Personal loans   |   |  Personal loans          |
               |  Student loans    |   |  Student loans           |
               +-------------------+   +---------------------------+
```

## 9. How Is the Loan Amount Determined

The loan amount is determined by several factors, including the borrower's income, debt levels, credit score, and the purpose of the loan.

How it works: Lenders calculate the maximum amount a borrower can afford based on their income and existing debt obligations. For secured loans, the loan amount is also limited by the value of the collateral (loan-to-value ratio). The lender ensures the borrower can make monthly payments without financial strain.

```
LOAN AMOUNT DETERMINATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   FACTOR 1: INCOME AND DEBT                                                │
    │   ├── Debt-to-Income Ratio (DTI)                                          │
    │   ├── DTI = Total Monthly Debt Payments / Gross Monthly Income            │
    │   ├── Maximum DTI typically 36-43%                                        │
    │   └── Lower DTI = Higher loan amount                                      │
    │                                                                             │
    │   FACTOR 2: CREDIT SCORE                                                   │
    │   ├── Higher score = Higher loan amount                                  │
    │   ├── Excellent (750+): Best terms                                       │
    │   ├── Good (700-749): Good terms                                         │
    │   ├── Fair (650-699): Acceptable terms                                   │
    │   └── Poor (<650): Limited options                                       │
    │                                                                             │
    │   FACTOR 3: COLLATERAL VALUE (Secured Loans)                             │
    │   ├── Loan-to-Value Ratio (LTV)                                          │
    │   ├── LTV = Loan Amount / Collateral Value                               │
    │   ├── Typical LTV: 80% (mortgage)                                        │
    │   ├── Lower LTV = Lower risk                                             │
    │   └── Higher LTV = Higher interest rate                                 │
    │                                                                             │
    │   FACTOR 4: LOAN PURPOSE                                                    │
    │   ├── Mortgages: Based on home value                                     │
    │   ├── Auto loans: Based on car value                                     │
    │   ├── Student loans: Based on cost of attendance                         │
    │   └── Business loans: Based on business revenue                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 10. What Is Interest

Interest is the cost of borrowing money. It is the fee the borrower pays to the lender for the use of funds. Interest is expressed as an annual percentage of the principal (loan amount).

How it works: The lender forgoes the use of their money while the borrower uses it. Interest compensates the lender for this opportunity cost, inflation, and the risk of default. The interest rate reflects the time value of money and the perceived risk of the borrower.

```
INTEREST EXPLANATION

                         +---------------------------+
                         |         LENDER            |
                         |       (Bank)              |
                         +-------------+-------------+
                                       |
                                       | Lends $10,000
                                       | For 1 year
                                       ▼
                         +---------------------------+
                         |        BORROWER           |
                         +-------------+-------------+
                                       |
                                       | Repays $10,000 + $500
                                       | Total: $10,500
                                       ▼
                         +---------------------------+
                         |         LENDER            |
                         +---------------------------+

    Interest = $500 (5% of $10,000)

    COMPONENTS OF INTEREST:
    +---------------------------+
    | 1. Cost of funds: What the lender pays for money
    | 2. Operating costs: Loan processing, administration
    | 3. Risk premium: Compensation for default risk
    | 4. Profit margin: Lender's earnings
    | 5. Inflation: Preserving purchasing power
    +---------------------------+
```

## 11. How Is Loan Interest Calculated

Loan interest is calculated using different methods depending on the loan type. The two most common methods are simple interest and compound interest, with amortization being the most common for installment loans.

How it works: Simple interest is calculated only on the principal. Compound interest is calculated on the principal plus any accumulated interest. Most installment loans (mortgages, auto loans) use amortization—a calculation that determines equal monthly payments covering both interest and principal over the loan term.

```
INTEREST CALCULATION METHODS

    METHOD 1: SIMPLE INTEREST
    I = P × r × t
    I = Interest
    P = Principal
    r = Annual interest rate (decimal)
    t = Time (in years)

    Example: $10,000 loan at 5% for 3 years
    I = $10,000 × 0.05 × 3 = $1,500
    Total Repayment = $11,500

    METHOD 2: COMPOUND INTEREST
    A = P × (1 + r/n)^(n×t)
    A = Total amount
    P = Principal
    r = Annual interest rate (decimal)
    n = Number of compounding periods per year
    t = Time (in years)

    Example: $10,000 at 5% compounded monthly for 3 years
    A = $10,000 × (1 + 0.05/12)^(12×3) = $11,614
    Interest = $1,614


    METHOD 3: AMORTIZATION (Installment Loans)
    PMT = P × [r(1+r)^n] / [(1+r)^n - 1]
    PMT = Monthly payment
    P = Principal
    r = Monthly interest rate (annual rate/12)
    n = Total number of payments

    Example: $100,000 loan at 6% for 30 years (360 months)
    Monthly interest rate = 0.06/12 = 0.005
    PMT = $100,000 × [0.005(1.005)^360] / [(1.005)^360 - 1]
    PMT = $599.55

    Payment Schedule:
    +-------------------------------------------------+
    | Month | Payment | Interest | Principal | Balance |
    |------|---------|----------|-----------|---------|
    | 1     | $599.55 | $500.00  | $99.55    | $99,900 |
    | 2     | $599.55 | $499.50  | $100.05   | $99,800 |
    | 3     | $599.55 | $499.00  | $100.55   | $99,699 |
    | ...   |         |          |           |         |
    | 360   | $599.55 | $2.99    | $596.56   | $0      |
    +-------------------------------------------------+
    (Interest portion decreases over time)
```

## 12. What Are Fixed and Variable Interest Rates

Fixed interest rates remain constant throughout the loan term. Variable (adjustable) rates change based on an underlying benchmark index.

How it works: Fixed rates provide payment certainty—the borrower knows exactly what their monthly payment will be for the entire term. Variable rates start lower but can increase or decrease based on market conditions, making payments unpredictable. Borrowers choose based on their risk tolerance and expectations for future interest rates.

```
FIXED VS VARIABLE RATES

                         +---------------------------+
                         |    FIXED RATE LOAN        |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  RATE STAYS SAME  |   |  PAYMENT PREDICTABLE      |
               |  Throughout term  |   |  Easy to budget           |
               |  No surprises     |   |  Higher initial rate      |
               |  Good for long    |   |  Protection from rising   |
               |  term planning   |   |  rates                    |
               +-------------------+   +---------------------------+


                         +---------------------------+
                         |  VARIABLE RATE LOAN       |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  RATE CAN CHANGE  |   |  PAYMENT FLUCTUATES       |
               |  Based on index   |   |  Harder to budget         |
               |  (SOFR, Prime)    |   |  Lower initial rate       |
               |  Good for short   |   |  Risk of rate increases   |
               |  term borrowing   |   |  or decreases             |
               +-------------------+   +---------------------------+


    VARIABLE RATE COMPONENTS:
    +---------------------------+
    | Index Rate (e.g., SOFR) + Margin = Fully Indexed Rate
    | Example: SOFR (4.50%) + Margin (2.00%) = 6.50%
    | Rate adjusts periodically (monthly, quarterly, annually)
    | Rate caps limit increases (per adjustment and lifetime)
    +---------------------------+
```

## 13. What Is the Loan Repayment Process

Loan repayment is the process by which the borrower pays back the principal and interest according to the loan agreement. Repayments are typically made in regular installments over the loan term.

How it works: The borrower makes scheduled payments (monthly, bi-weekly, or quarterly) to the lender. Each payment covers both interest and principal (in varying proportions). The lender applies the payment to the outstanding balance, reducing it until the loan is fully repaid.

```
LOAN REPAYMENT PROCESS

    +-------------------------------------------------+
    |  Borrower makes scheduled payment               |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Lender applies payment:                        |
    |  1. Interest for the period                     |
    |  2. Principal (remaining amount)                |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Outstanding balance is reduced                 |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Statement generated showing remaining balance  |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Process repeats each payment period            |
    |  until balance reaches zero                     |
    +-------------------------------------------------+
```

## 14. What Are Loan Installments (EMIs)

Equated Monthly Installments (EMIs) are fixed payments made by the borrower to the lender at a specified date each month. Each EMI includes both principal and interest.

How it works: The EMI amount is calculated so that the loan is fully repaid by the end of the term. Early in the loan term, a larger portion of the EMI goes toward interest. Later, more goes toward principal. This is called amortization.

```
EMI STRUCTURE

    +-------------------------------------------------+
    |  LOAN: $100,000 at 6% for 30 years              |
    |  Monthly EMI: $599.55                           |
    +-------------------------------------------------+

    Early Years (First Payment):
    +-------------------------------------------------+
    |  Payment: $599.55                               |
    |  Interest: $500.00 (83% of payment)             |
    |  Principal: $99.55 (17% of payment)             |
    |  Remaining: $99,900.45                          |
    +-------------------------------------------------+

    Middle Years (Year 15):
    +-------------------------------------------------+
    |  Payment: $599.55                               |
    |  Interest: $250.00 (42% of payment)             |
    |  Principal: $349.55 (58% of payment)            |
    |  Remaining: ~$50,000                            |
    +-------------------------------------------------+

    Final Years (Last Payment):
    +-------------------------------------------------+
    |  Payment: $599.55                               |
    |  Interest: $2.99 (0.5% of payment)              |
    |  Principal: $596.56 (99.5% of payment)          |
    |  Remaining: $0                                  |
    +-------------------------------------------------+
```

## 15. What Happens If a Borrower Misses Payments

Missing payments triggers a series of consequences, starting with fees and potentially ending with default and legal action.

How it works: Late payments incur fees and penalties. The lender reports late payments to credit bureaus, damaging the borrower's credit score. Continued non-payment leads to default, where the lender can demand full repayment, seize collateral (if secured), or pursue legal action. The process typically follows a defined timeline.

```
MISSED PAYMENT TIMELINE

    +-------------------------------------------------+
    |  DAY 1: Payment due                             |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  GRACE PERIOD (3-15 days): No penalty           |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  DAY 30: Late payment notice                    |
    |  - Late fee charged                             |
    |  - Reported to credit bureaus (30+ days late)   |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  DAY 60: Second notice                          |
    |  - Additional fees                              |
    |  - Credit score significantly impacted          |
    |  - Collection calls begin                       |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  DAY 90: Default notice                         |
    |  - Loan may be declared in default             |
    |  - Full balance may become due                  |
    |  - Sent to collections                          |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  DAY 120+: Legal action                         |
    |  - Lawsuit filed (unsecured)                    |
    |  - Foreclosure begins (secured)                 |
    |  - Wage garnishment possible                    |
    |  - Asset seizure                               |
    +-------------------------------------------------+
```

## 16. What Is Loan Default

Loan default occurs when a borrower fails to meet the legal obligations of the loan agreement, typically by missing multiple consecutive payments. Default is the final stage of non-payment before legal action.

How it works: Default triggers the lender's right to demand full repayment of the outstanding balance (acceleration). For secured loans, the lender can seize and sell the collateral. For unsecured loans, the lender can sue the borrower, obtain a judgment, and pursue wage garnishment or asset seizure. Default severely damages credit scores and can remain on credit reports for 7 years.

```
DEFAULT CONSEQUENCES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CONSEQUENCE 1: CREDIT DAMAGE                                              │
    │   ├── Credit score drops significantly (100-200+ points)                   │
    │   ├── Default remains on credit report for 7 years                         │
    │   ├── Difficulty obtaining future credit                                   │
    │   └── Higher interest rates on future loans                               │
    │                                                                             │
    │   CONSEQUENCE 2: SECURED LOAN (Collateral Seizure)                         │
    │   ├── Mortgage: Foreclosure                                                │
    │   ├── Auto loan: Repossession                                              │
    │   ├── Asset sold by lender                                                │
    │   ├── Deficiency judgment if sale < balance                               │
    │   └── Borrower loses the asset                                            │
    │                                                                             │
    │   CONSEQUENCE 3: UNSECURED LOAN (Legal Action)                            │
    │   ├── Lawsuit filed                                                       │
    │   ├── Court judgment obtained                                             │
    │   ├── Wage garnishment (up to 25% of wages)                               │
    │   ├── Bank account levy                                                  │
    │   └── Property lien                                                       │
    │                                                                             │
    │   CONSEQUENCE 4: FINANCIAL COSTS                                           │
    │   ├── Late fees and penalties                                             │
    │   ├── Legal fees and court costs                                          │
    │   ├── Collection agency fees                                              │
    │   └── Interest continues to accrue                                        │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 17. How Do Banks Create Money Through Lending

Banks create money when they issue loans. This is the most important function of the banking system and the foundation of money creation.

How it works: When a bank approves a loan, it credits the borrower's deposit account with the loan amount. This creates a new deposit that did not exist before. No existing deposits are used. The bank creates a new asset (loan receivable) and a new liability (the borrower's deposit). This expands the money supply by the full amount of the loan.

```
MONEY CREATION THROUGH LENDING

                         BEFORE LOAN:

                         +---------------------------+
                         |    BANK BALANCE SHEET     |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  ASSETS           |   |  LIABILITIES              |
               |  Reserves: $10M   |   |  Deposits: $100M          |
               |  Loans: $0        |   |  Equity: $10M             |
               +-------------------+   +---------------------------+

    Money Supply = $100M (Deposits)
    Reserve Ratio = 10%


                         AFTER $20M LOAN:

                         +---------------------------+
                         |    BANK BALANCE SHEET     |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  ASSETS           |   |  LIABILITIES              |
               |  Reserves: $10M   |   |  Deposits: $120M          |
               |  Loans: $20M     |   |  Equity: $10M             |
               +-------------------+   +---------------------------+

    Money Supply = $120M (+$20M CREATED)
    Reserve Ratio = 10%
    Required Reserves = $12M (shortfall of $2M)

    KEY INSIGHT: New money was created from nothing.
    No existing deposit was used.
    The loan created a new deposit.
```

## 18. What Is Fractional Reserve Banking

Fractional reserve banking is a system where banks are required to hold only a fraction of their deposits as reserves. The remaining deposits can be lent out, creating new money.

How it works: A bank receives a $100 deposit. The reserve requirement is 10%. The bank holds $10 as reserves and lends out $90. The $90 is deposited into another bank, which holds $9 as reserves and lends out $81. This process continues, multiplying the original deposit into a larger total money supply.

```
FRACTIONAL RESERVE BANKING PROCESS

    +-------------------------------------------------+
    |  Initial Deposit: $100,000                      |
    |  Reserve Requirement: 10%                       |
    |  Money Multiplier: 1 / 0.10 = 10               |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  Bank A:                                        |
    |  Deposits: +$100,000                            |
    |  Reserves: +$10,000 (10%)                       |
    |  Loan: +$90,000 (90%)                           |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Bank B:                                         |
    |  Deposits: +$90,000                             |
    |  Reserves: +$9,000 (10%)                        |
    |  Loan: +$81,000 (90%)                           |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Bank C:                                         |
    |  Deposits: +$81,000                             |
    |  Reserves: +$8,100 (10%)                        |
    |  Loan: +$72,900 (90%)                           |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  Process continues...                           |
    |  Total Deposits Created: $1,000,000            |
    |  Total Reserves Held: $100,000                 |
    |  Total Loans Made: $900,000                    |
    +-------------------------------------------------+

    Money Multiplier = 1 / Reserve Requirement Ratio
    = 1 / 0.10 = 10

    Total Money Created = Initial Deposit × Multiplier
    = $100,000 × 10 = $1,000,000
```

## 19. Why Don't Banks Need to Keep All Deposited Money

Banks do not need to keep all deposited money because depositors do not all withdraw at the same time. This is the foundation of fractional reserve banking.

How it works: Under normal conditions, only a small percentage of depositors withdraw their money on any given day. Banks use this predictability to lend out most deposits while keeping enough reserves to meet daily withdrawal demands. This is called the "law of large numbers"—with many depositors, daily withdrawal patterns are predictable.

```
WHY FRACTIONAL RESERVES WORK

    +-------------------------------------------------+
    |  10,000 DEPOSITORS EACH HAVE $10,000           |
    |  Total Deposits: $100,000,000                  |
    +-------------------------------------------------+

    Normal Daily Activity:
    +-------------------------------------------------+
    |  Deposits: $5,000,000 (500 depositors)          |
    |  Withdrawals: $4,500,000 (450 depositors)       |
    |  Net Change: +$500,000                          |
    |  Reserves Needed: $500,000 (for net outflow)    |
    +-------------------------------------------------+

    If bank keeps 10% reserves ($10,000,000):
    +-------------------------------------------------+
    |  Even if 10% of depositors withdraw ($10M)     |
    |  Bank has $10M reserves = covers all withdrawals|
    |  No need to sell assets or borrow              |
    |  System remains stable                         |
    +-------------------------------------------------+

    Why It Works:
    +-------------------------------------------------+
    |  Law of Large Numbers: Withdrawals predictable  |
    |  Deposit Insurance: Prevents panic withdrawals  |
    |  Central Bank: Last resort lending              |
    |  Bank Reserves: Buffer for normal variation     |
    +-------------------------------------------------+
```

## 20. How Does Money Creation Increase the Money Supply

Money creation through lending multiplies the initial monetary base into a larger total money supply. This is known as the money multiplier effect.

How it works: The central bank creates base money (currency and reserves). Commercial banks use this base money to create new deposits through lending. Each deposit creates the potential for another loan, which creates another deposit. The total money supply becomes a multiple of the base money.

```
MONEY SUPPLY MULTIPLICATION

                    CENTRAL BANK CREATES BASE MONEY
                              ($100,000)
                                    │
                                    ▼
                    +---------------------------+
                    |   COMMERCIAL BANKS        |
                    |   Create deposits         |
                    |   through lending         |
                    +---------------------------+
                                    │
                                    ▼
                +-------------------------------------------------+
                |   MONEY MULTIPLIER EFFECT                      |
                |                                                 |
                |   Deposit 1: $100,000   Reserve: $10,000       |
                |                       ↓ Loan: $90,000          |
                |                                                 |
                |   Deposit 2: $90,000    Reserve: $9,000        |
                |                       ↓ Loan: $81,000          |
                |                                                 |
                |   Deposit 3: $81,000    Reserve: $8,100        |
                |                       ↓ Loan: $72,900          |
                |                                                 |
                |   ... continues until $1,000,000 total         |
                |                                                 |
                |   Total Deposits: $1,000,000                   |
                |   Total Reserves: $100,000                     |
                |   Total Loans: $900,000                        |
                |   Money Multiplier: 10                         |
                +-------------------------------------------------+
                                    │
                                    ▼
                    +---------------------------+
                    |   MONEY SUPPLY INCREASES  |
                    |   From $100,000 to $1M    |
                    |   (10x multiplication)    |
                    +---------------------------+
```

## 21. What Limits a Bank's Ability to Create Money

Banks face several constraints that limit their ability to create money through lending.

```
LIMITS ON MONEY CREATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   LIMIT 1: RESERVE REQUIREMENTS                                             │
    │   ├── Banks must hold reserves against deposits                           │
    │   ├── Reserve ratio limits lending capacity                               │
    │   ├── Excess reserves determine lending power                             │
    │   └── Higher requirements = Less money creation                           │
    │                                                                             │
    │   LIMIT 2: CAPITAL REQUIREMENTS                                            │
    │   ├── Banks must maintain minimum capital ratios                          │
    │   ├── Lending increases risk-weighted assets                              │
    │   ├── More lending requires more capital                                 │
    │   └── Basel III capital standards limit lending                          │
    │                                                                             │
    │   LIMIT 3: CREDITWORTHY BORROWERS                                          │
    │   ├── Banks cannot lend to uncreditworthy borrowers                      │
    │   ├── Requires qualified borrowers with capacity to repay                │
    │   ├── Limited number of bankable projects                                 │
    │   └── Credit standards restrict lending                                   │
    │                                                                             │
    │   LIMIT 4: LIQUIDITY REQUIREMENTS                                          │
    │   ├── LCR (Liquidity Coverage Ratio)                                     │
    │   ├── NSFR (Net Stable Funding Ratio)                                    │
    │   ├── Banks must maintain liquid assets                                  │
    │   └── Restricts long-term illiquid lending                               │
    │                                                                             │
    │   LIMIT 5: MARKET DEMAND FOR LOANS                                         │
    │   ├── Banks cannot lend if no one wants to borrow                        │
    │   ├── Interest rates affect loan demand                                  │
    │   ├── Economic conditions affect borrowing                                │
    │   └── Demand constraints may limit lending                               │
    │                                                                             │
    │   LIMIT 6: CENTRAL BANK POLICY                                             │
    │   ├── Policy rate affects lending costs                                  │
    │   ├── Open market operations affect reserves                             │
    │   ├── Quantitative easing increases reserves                             │
    │   └── Monetary policy influences lending volume                          │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 22. What Is the Role of Central Banks in Money Creation

Central banks are the ultimate source of money creation. They create base money (currency and reserves) and set the rules that determine how commercial banks create broad money.

How it works: The central bank controls the monetary base through open market operations, reserve requirements, and the policy rate. Commercial banks use this base money to create deposits through lending. The central bank supervises the banking system to ensure prudent lending. In times of crisis, the central bank acts as lender of last resort.

```
CENTRAL BANK ROLES IN MONEY CREATION

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   ROLE 1: CREATE BASE MONEY                                                │
    │   ├── Issue currency (notes and coins)                                     │
    │   ├── Create reserves through open market operations                      │
    │   ├── Quantitative easing expands base money                             │
    │   └── Base money is the foundation of money creation                     │
    │                                                                             │
    │   ROLE 2: SET MONETARY POLICY                                              │
    │   ├── Policy rate influences lending costs                               │
    │   ├── Reserve requirements limit money creation                          │
    │   ├── Open market operations adjust reserves                             │
    │   └── Forward guidance shapes expectations                               │
    │                                                                             │
    │   ROLE 3: SUPERVISE BANKS                                                 │
    │   ├── Ensure prudent lending practices                                  │
    │   ├── Enforce capital requirements                                       │
    │   ├── Conduct stress tests                                               │
    │   └── Prevent excessive money creation                                  │
    │                                                                             │
    │   ROLE 4: LENDER OF LAST RESORT                                           │
    │   ├── Provide emergency liquidity                                        │
    │   ├── Prevent bank runs                                                  │
    │   ├── Maintain financial stability                                      │
    │   └── Support money creation during crises                              │
    │                                                                             │
    │   ROLE 5: TARGET INFLATION                                                 │
    │   ├── Control money supply to meet inflation target                     │
    │   ├── Prevent excessive money creation leading to inflation             │
    │   ├── Prevent insufficient money creation leading to deflation         │
    │   └── Balance money creation with economic growth                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 23. How Do Reserve Requirements Affect Lending

Reserve requirements determine how much banks can lend and therefore how much money can be created.

How it works: The reserve requirement ratio sets the minimum fraction of deposits that banks must hold as reserves. A higher ratio reduces the money multiplier and limits lending. A lower ratio increases the multiplier and allows more lending. The central bank uses reserve requirements as a tool to control money creation.

```
RESERVE REQUIREMENT IMPACT ON LENDING

    +-------------------------------------------------+
    |  RESERVE REQUIREMENT = 10%                      |
    |  Money Multiplier = 1 / 0.10 = 10              |
    |  Initial Deposit: $100,000                     |
    |  Total Money Created: $1,000,000              |
    +-------------------------------------------------+
                         │
                         ▼
    +-------------------------------------------------+
    |  RESERVE REQUIREMENT = 20%                      |
    |  Money Multiplier = 1 / 0.20 = 5               |
    |  Initial Deposit: $100,000                     |
    |  Total Money Created: $500,000                 |
    +-------------------------------------------------+

    Impact: Higher requirement reduces lending capacity by 50%

    +-------------------------------------------------+
    |  RESERVE REQUIREMENT = 0%                       |
    |  Money Multiplier = Infinite (theoretically)   |
    |  Initial Deposit: $100,000                     |
    |  Total Money Created: Unlimited                |
    +-------------------------------------------------+

    Impact: Zero requirement removes lending limit
    (Central bank uses interest on reserves instead)
```

## 24. How Do Interest Rates Influence Loan Demand

Interest rates are the price of borrowing. Higher rates reduce loan demand, while lower rates increase loan demand.

How it works: When rates are high, the cost of borrowing is high, making loans less attractive. Households delay major purchases. Businesses postpone investments. When rates are low, borrowing becomes cheaper, encouraging households and businesses to take loans. The central bank uses interest rates to influence borrowing and spending in the economy.

```
INTEREST RATE EFFECT ON LOAN DEMAND

                         +---------------------------+
                         |   HIGH INTEREST RATES     |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  Borrowing Cost   |   |  Lower Loan Demand        |
               |  High             |   |  - Fewer mortgages        |
               |  Less attractive  |   |  - Less business loans    |
               |  Discourages      |   |  - Reduced spending       |
               |  borrowing        |   |  - Slower money creation  |
               +-------------------+   +---------------------------+


                         +---------------------------+
                         |   LOW INTEREST RATES      |
                         +-------------+-------------+
                                       |
                         +-------------+-------------+
                         |                           |
                         ▼                           ▼
               +-------------------+   +---------------------------+
               |  Borrowing Cost   |   |  Higher Loan Demand       |
               |  Low              |   |  - More mortgages         |
               |  More attractive  |   |  - More business loans    |
               |  Encourages       |   |  - Increased spending     |
               |  borrowing        |   |  - Faster money creation  |
               +-------------------+   +---------------------------+
```

## 25. How Do Loans Affect Inflation

Loans affect inflation by increasing the money supply. When banks create new money through lending, they increase the total amount of money in the economy. If this increase exceeds economic growth, it can lead to inflation.

How it works: More money in the economy means more spending power. If the supply of goods and services does not increase proportionally, prices rise (inflation). Excessive lending can cause demand-pull inflation. Central banks monitor lending and adjust policy to keep inflation at target levels.

```
LOANS AND INFLATION CONNECTION

    +-------------------------------------------------+
    |  BANK CREATES NEW MONEY THROUGH LENDING         |
    |  Money Supply Increases                         |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  ECONOMIC IMPACT                                |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  MORE MONEY IN ECONOMY                         |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  INCREASED SPENDING                             |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  IF GOODS SUPPLY CONSTANT: PRICES RISE         |
    |  (Demand-Pull Inflation)                       |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  BALANCE NEEDED:                                |
    |  Money creation = Economic growth              |
    |  Inflation stable at 2%                        |
    +-------------------------------------------------+
    |  TOO MUCH LENDING:                              |
    |  Money creation > Economic growth              |
    |  Inflation rises above target                  |
    +-------------------------------------------------+
    |  TOO LITTLE LENDING:                            |
    |  Money creation < Economic growth              |
    |  Deflation risk, slow growth                   |
    +-------------------------------------------------+
```

## 26. How Do Loans Support Economic Growth

Loans are essential for economic growth. They enable investment, consumption, and entrepreneurship that would not be possible with existing savings alone.

How it works: Loans channel funds from savers to borrowers who can use them productively. Businesses invest in new equipment, technology, and expansion. Households buy homes and cars. Entrepreneurs start new ventures. This increases production, employment, and income. The economy grows as resources are allocated to their most productive uses.

```
LOANS SUPPORTING ECONOMIC GROWTH

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CHANNEL 1: BUSINESS INVESTMENT                                           │
    │   ├── Loans fund capital expenditure (CAPEX)                              │
    │   ├── Businesses buy equipment, machinery, technology                     │
    │   ├── Increases productivity and efficiency                              │
    │   └── Expands production capacity                                        │
    │                                                                             │
    │   CHANNEL 2: HOUSEHOLD CONSUMPTION                                        │
    │   ├── Mortgages enable home ownership                                    │
    │   ├── Auto loans enable vehicle purchases                                │
    │   ├── Student loans fund education                                       │
    │   └── Personal loans support consumption                                 │
    │                                                                             │
    │   CHANNEL 3: ENTREPRENEURSHIP                                             │
    │   ├── Startups need funding for innovation                               │
    │   ├── Small business loans enable new ventures                           │
    │   ├── Job creation through new businesses                               │
    │   └── Economic diversification                                           │
    │                                                                             │
    │   CHANNEL 4: JOB CREATION                                                 │
    │   ├── Investment creates employment                                      │
    │   ├── New businesses hire workers                                        │
    │   ├── Existing businesses expand workforce                              │
    │   └── Income generation through employment                              │
    │                                                                             │
    │   CHANNEL 5: MULTIPLIER EFFECT                                            │
    │   ├── One loan creates multiple economic transactions                   │
    │   ├── Spending becomes income for others                                 │
    │   ├── Income leads to more spending                                      │
    │   └── Economic activity multiplies                                      │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 27. What Are the Risks of Excessive Lending

Excessive lending occurs when banks create too much money too quickly, leading to economic imbalances and financial instability.

How it works: Excessive lending can cause asset bubbles (housing, stocks), over-indebtedness, and inflation. Borrowers take on debt they cannot repay. Banks become over-leveraged. When the cycle reverses, defaults rise, banks fail, and the economy contracts. This is the boom-bust cycle.

```
RISKS OF EXCESSIVE LENDING

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   RISK 1: ASSET BUBBLES                                                    │
    │   ├── Too much money chasing assets                                       │
    │   ├── Housing prices inflate                                              │
    │   ├── Stock market overvaluation                                          │
    │   └── Bubbles eventually burst                                           │
    │                                                                             │
    │   RISK 2: OVER-INDEBTEDNESS                                                │
    │   ├── Borrowers take on too much debt                                    │
    │   ├── Debt service consumes income                                       │
    │   ├── Defaults rise when conditions change                                │
    │   └── Household and business distress                                    │
    │                                                                             │
    │   RISK 3: BANK INSTABILITY                                                 │
    │   ├── Banks become over-leveraged                                        │
    │   ├── Loan losses erode capital                                          │
    │   ├── Bank runs when confidence fails                                    │
    │   └── Bank failures lead to credit crunch                               │
    │                                                                             │
    │   RISK 4: INFLATION                                                       │
    │   ├── Too much money chasing too few goods                                │
    │   ├── Prices rise                                                       │
    │   ├── Purchasing power erodes                                            │
    │   └── Central bank must intervene                                       │
    │                                                                             │
    │   RISK 5: FINANCIAL CRISIS                                                │
    │   ├── Boom-bust cycle                                                    │
    │   ├── Excessive lending → asset bubble → crash                          │
    │   ├── Bank failures → credit freeze                                     │
    │   └── Recession follows                                                  │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 28. What Causes Bad Loans (Non-Performing Loans)

Non-Performing Loans (NPLs) are loans where the borrower has not made payments for 90 days or more. NPLs are a major concern for banks and regulators.

How it works: Borrowers default for various reasons: loss of income, business failure, economic downturn, or excessive debt. When borrowers cannot repay, loans become non-performing. Banks must set aside provisions (reserves) for expected losses, reducing profitability. High NPL ratios indicate a distressed banking sector.

```
CAUSES OF NON-PERFORMING LOANS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   CAUSE 1: BORROWER DISTRESS                                               │
    │   ├── Job loss or income reduction                                        │
    │   ├── Business failure                                                    │
    │   ├── Health emergencies                                                  │
    │   └── Divorce or family issues                                            │
    │                                                                             │
    │   CAUSE 2: ECONOMIC DOWNTURN                                               │
    │   ├── Recession reduces income                                           │
    │   ├── Unemployment rises                                                 │
    │   ├── Business revenues fall                                              │
    │   └── Widespread defaults                                                │
    │                                                                             │
    │   CAUSE 3: POOR UNDERWRITING                                               │
    │   ├── Lending to uncreditworthy borrowers                                 │
    │   ├── Inadequate income verification                                     │
    │   ├── Overly optimistic assumptions                                      │
    │   └── Loose lending standards                                            │
    │                                                                             │
    │   CAUSE 4: ASSET BUBBLE BURST                                              │
    │   ├── Housing price crash                                                │
    │   ├── Borrowers underwater (loan > asset value)                          │
    │   ├── Strategic defaults                                                 │
    │   └── Collateral value declines                                          │
    │                                                                             │
    │   CAUSE 5: INTEREST RATE RISES                                             │
    │   ├── Variable rate loans become unaffordable                            │
    │   ├── Higher payments strain borrowers                                   │
    │   ├── Defaults on adjustable rate mortgages                              │
    │   └── Refinancing becomes impossible                                     │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 29. How Do Banks Manage Loan Risk

Banks use various tools and strategies to manage the risk of borrower default.

How it works: Before lending, banks assess borrower risk through credit checks, income verification, and collateral valuation. After lending, they monitor payments and financial health. They diversify across borrowers, industries, and geographies. They set aside reserves for expected losses. They require collateral for large loans. They use loan covenants to protect their interests.

```
LOAN RISK MANAGEMENT TOOLS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   TOOL 1: UNDERWRITING STANDARDS                                           │
    │   ├── Credit scoring and analysis                                         │
    │   ├── Debt-to-income limits                                              │
    │   ├── Loan-to-value limits                                               │
    │   └── Income verification                                                │
    │                                                                             │
    │   TOOL 2: COLLATERAL REQUIREMENTS                                         │
    │   ├── Secured by assets (property, equipment, deposits)                  │
    │   ├── Lien on collateral                                                │
    │   ├── Foreclosure or repossession rights                                 │
    │   └── Guarantees from third parties                                     │
    │                                                                             │
    │   TOOL 3: DIVERSIFICATION                                                  │
    │   ├── Across borrowers (not concentrated in one customer)                │
    │   ├── Across industries (not concentrated in oil, real estate)           │
    │   └── Across geographies                                                │
    │                                                                             │
    │   TOOL 4: LOAN LOSS RESERVES (PROVISIONS)                                 │
    │   ├── Reserve for expected losses                                       │
    │   ├── Based on historical default rates                                 │
    │   ├── Adjusted for economic conditions                                  │
    │   └── CECL (Current Expected Credit Losses) standard                   │
    │                                                                             │
    │   TOOL 5: LOAN COVENANTS                                                   │
    │   ├── Financial covenants (maintain ratios)                               │
    │   ├── Reporting requirements                                              │
    │   ├── Restrictions on additional borrowing                               │
    │   └── Triggers for early repayment                                       │
    │                                                                             │
    │   TOOL 6: CAPITAL REQUIREMENTS                                            │
    │   ├── Equity absorbs unexpected losses                                   │
    │   ├── Higher capital = greater loss absorption                           │
    │   └── Regulatory minimums (4.5% CET1)                                   │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 30. What Is Creditworthiness

Creditworthiness is a lender's assessment of a borrower's ability and willingness to repay a loan. It determines whether a borrower qualifies for a loan and the terms offered.

How it works: Creditworthiness is evaluated using credit reports, credit scores, income, assets, and debt levels. Lenders look for evidence of responsible financial behavior and capacity to repay. Higher creditworthiness results in lower interest rates and better loan terms.

```
CREDITWORTHINESS ASSESSMENT

    +-------------------------------------------------+
    |  CREDIT SCORE (FICO)                            |
    |  Excellent (750+): Best rates                   |
    |  Good (700-749): Good rates                     |
    |  Fair (650-699): Acceptable rates               |
    |  Poor (600-649): High rates                    |
    |  Bad (<600): May be declined                   |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  DEBT-TO-INCOME RATIO (DTI)                     |
    |  DTI = Total Monthly Debt Payments / Income     |
    |  < 36%: Excellent                              |
    |  36-43%: Good                                  |
    |  43-50%: Marginal                             |
    |  > 50%: High risk                             |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  INCOME AND EMPLOYMENT                          |
    |  Stable income (2+ years at same job)          |
    |  Sufficient income to cover payments           |
    |  Rising income trend                           |
    |  Low risk of job loss                          |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  EXISTING DEBT OBLIGATIONS                       |
    |  Few existing loans                             |
    |  Low credit utilization (credit cards)         |
    |  On-time payment history                       |
    |  No recent defaults or bankruptcies            |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  ASSETS AND SAVINGS                             |
    |  Substantial savings/emergency fund            |
    |  Investment portfolio                         |
    |  Real estate or other assets                  |
    |  Ability to handle income disruption           |
    +-------------------------------------------------+
```

## 31. What Is a Credit Score

A credit score is a numerical representation of a borrower's creditworthiness, based on their credit history. It is used by lenders to assess the risk of lending.

How it works: Credit scores are calculated using data from credit reports, including payment history, amounts owed, length of credit history, credit mix, and new credit. The most common score is FICO, ranging from 300 to 850. Higher scores indicate lower risk and result in better loan terms.

```
CREDIT SCORE COMPONENTS (FICO)

    +-------------------------------------------------+
    |  PAYMENT HISTORY (35%)                          |
    |  On-time payments vs late payments              |
    |  Public records (bankruptcies, judgments)      |
    |  Collection accounts                           |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  AMOUNTS OWED (30%)                             |
    |  Total debt                                     |
    |  Credit utilization ratio (30% or less ideal)   |
    |  Loan balances                                  |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  LENGTH OF CREDIT HISTORY (15%)                 |
    |  Age of oldest account                          |
    |  Average age of all accounts                   |
    |  Age of newest account                         |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  CREDIT MIX (10%)                               |
    |  Variety of credit types (cards, mortgage,     |
    |  auto, student loans)                         |
    +-------------------------------------------------+

    +-------------------------------------------------+

    +-------------------------------------------------+
    |  NEW CREDIT (10%)                               |
    |  Number of recent inquiries                    |
    |  Number of recently opened accounts            |
    |  Time since last inquiry                      |
    +-------------------------------------------------+
```

## 32. How Do Banks Evaluate Borrowers

Banks use a systematic process to evaluate borrowers and determine loan eligibility and terms.

How it works: The evaluation process involves credit checks, income verification, asset assessment, and risk analysis. Banks use both automated systems (credit scoring) and manual underwriting for complex cases. The result is a risk rating that determines whether to approve, the loan amount, and the interest rate.

```
BORROWER EVALUATION PROCESS

    +-------------------------------------------------+
    |  STEP 1: CREDIT CHECK                           |
    |  - Pull credit report                          |
    |  - Review credit score                        |
    |  - Check payment history                       |
    |  - Identify red flags (collections, judgments)|
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  STEP 2: INCOME VERIFICATION                    |
    |  - Pay stubs (2+ years)                        |
    |  - Tax returns (W-2, 1040)                    |
    |  - Bank statements                            |
    |  - Employer verification                      |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  STEP 3: ASSET VERIFICATION                     |
    |  - Bank accounts                              |
    |  - Investment accounts                        |
    |  - Real estate holdings                       |
    |  - Other assets                              |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  STEP 4: DEBT CALCULATION                       |
    |  - Total monthly debt payments                |
    |  - Debt-to-income ratio (DTI)                  |
    |  - Compare to maximum DTI (36-43%)            |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  STEP 5: COLLATERAL EVALUATION (Secured)       |
    |  - Appraisal of asset                         |
    |  - Loan-to-value ratio (LTV)                  |
    |  - Collateral quality                        |
    +--------------------+----------------------------+
                         |
                         ▼
    +-------------------------------------------------+
    |  STEP 6: UNDERWRITING DECISION                  |
    |  - Approve, decline, or counter-offer         |
    |  - Determine loan amount                     |
    |  - Set interest rate                         |
    |  - Establish terms and covenants             |
    +-------------------------------------------------+
```

## 33. What Is the Difference Between Lending Existing Money and Creating New Money

This is a fundamental distinction: when a bank lends existing deposits, it transfers purchasing power. When it creates new money through lending, it expands the money supply.

How it works: Lending existing money occurs when a bank uses funds from a depositor or other funding source to make a loan. This simply transfers the money from one account to another. Creating new money occurs when the bank issues a loan by crediting the borrower's account with a new deposit. This creates new money that did not exist before. Most bank lending creates new money.

```
LENDING EXISTING MONEY VS CREATING NEW MONEY

    LENDING EXISTING MONEY:
    +-------------------------------------------------+
    |  Bank uses depositor funds to make loan        |
    |  Funds transfer from depositor to borrower    |
    |  Money supply unchanged                       |
    |  Example: Using savings deposits             |
    +-------------------------------------------------+

    CREATING NEW MONEY:
    +-------------------------------------------------+
    |  Bank credits borrower's account with new     |
    |  deposit. No existing deposit is used.        |
    |  Money supply increases by loan amount        |
    |  Example: Most commercial bank lending        |
    +-------------------------------------------------+

    Comparison:

    +-------------------------------------------------+
    |  Aspect         | Existing Money   | New Money   |
    |-----------------|-----------------|-------------|
    | Source          | Depositor funds | Bank creates|
    | Money supply    | Unchanged        | Increases   |
    | Asset impact    | Depositor asset  | Bank loan   |
    |                 | decreases        | asset       |
    | Liability impact| Depositor        | Borrower    |
    |                 | liability        | deposit     |
    |                 | decreases        | liability   |
    |                 |                  | increases   |
    | Balance sheet   | Size unchanged   | Size grows  |
    +-------------------------------------------------+
```

## 34. How Does Loan Repayment Destroy Bank-Created Money

When a borrower repays a loan, the opposite of money creation occurs: money is destroyed. The borrower's deposit is debited, and the loan asset is reduced.

How it works: The borrower makes a payment from their deposit account. The bank debits the deposit (reducing the liability) and reduces the loan asset. The deposit disappears from the money supply. This is the primary mechanism for money destruction in the economy.

```
LOAN REPAYMENT MONEY DESTRUCTION

    BEFORE REPAYMENT:
    +-------------------------------------------------+
    |  Bank Assets                    | Liabilities   |
    |  Reserve: $10,000              | Deposits:     |
    |  Loans: $20,000                | $120,000       |
    |                                | Equity: $10,000|
    |  Money Supply: $120,000                          |
    +-------------------------------------------------+

    BORROWER REPAYS $5,000:
    +-------------------------------------------------+
    |  Bank Assets                    | Liabilities   |
    |  Reserve: $10,000              | Deposits:     |
    |  Loans: $15,000                | $115,000       |
    |                                | Equity: $10,000|
    |  Money Supply: $115,000                          |
    +-------------------------------------------------+

    RESULT:
    +-------------------------------------------------+
    |  Money supply decreased by $5,000              |
    |  Loan asset decreased by $5,000               |
    |  Deposit liability decreased by $5,000        |
    |  Money is destroyed                            |
    +-------------------------------------------------+
```

## 35. What Happens When a Loan Is Fully Repaid

When a loan is fully repaid, the money created when the loan was made is completely destroyed. The loan asset and deposit liability are both eliminated.

How it works: The final payment fully debits the borrower's deposit and reduces the loan balance to zero. The bank removes the loan from its books. The deposit created at loan origination is gone. The money supply returns to its pre-loan level (all else being equal). The bank earns the interest over the life of the loan.

```
FULL LOAN REPAYMENT

    LOAN ORIGINATION ($20,000 CREATED):
    +-------------------------------------------------+
    |  Bank Assets                    | Liabilities   |
    |  Reserve: $10,000              | Deposits:     |
    |  Loans: $20,000                | $120,000       |
    |                                | Equity: $10,000|
    +-------------------------------------------------+

    DURING REPAYMENT (Principal + Interest):
    +-------------------------------------------------+
    |  Borrower makes monthly payments                |
    |  Interest portion: Bank income (retained)      |
    |  Principal portion: Money destroyed           |
    |  Loan balance decreases                         |
    +-------------------------------------------------+

    FULLY REPAID:
    +-------------------------------------------------+
    |  Bank Assets                    | Liabilities   |
    |  Reserve: $10,000              | Deposits:     |
    |  Loans: $0                     | $100,000       |
    |                                | Equity: $14,000|
    |                                | (Original     |
    |                                |  equity +     |
    |                                |  interest)    |
    +-------------------------------------------------+

    Money Supply: $100,000 (returned to pre-loan level)
    Bank earned interest during the loan term
```

## 36. What Is the Complete Lifecycle of a Bank Loan

The complete lifecycle of a loan includes all stages from application to final repayment and closure.

```
COMPLETE LOAN LIFECYCLE

    STAGE 1: APPLICATION
    +-------------------------------------------------+
    |  Borrower applies for loan                      |
    |  Submits financial information                 |
    |  Specifies purpose and amount                  |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 2: UNDERWRITING
    +-------------------------------------------------+
    |  Bank evaluates borrower                        |
    |  Credit check, income verification              |
    |  Debt-to-income analysis                       |
    |  Collateral valuation (secured)                |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 3: APPROVAL
    +-------------------------------------------------+
    |  Loan approved or declined                     |
    |  Terms set (rate, amount, term, covenants)     |
    |  Offer extended to borrower                   |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 4: CLOSING
    +-------------------------------------------------+
    |  Borrower accepts offer                        |
    |  Legal documents signed                        |
    |  Loan agreement executed                       |
    |  Funds disbursed                              |
    |  New money created                            |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 5: SERVICING
    +-------------------------------------------------+
    |  Borrower makes regular payments               |
    |  Bank collects interest and principal          |
    |  Loan amortization proceeds                   |
    |  Interest portion declines over time          |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 6: MONITORING
    +-------------------------------------------------+
    |  Bank monitors payment performance             |
    |  Reviews borrower financial condition          |
    |  Identifies early warning signs                |
    |  Manages problem loans                        |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 7: REPAYMENT
    +-------------------------------------------------+
    |  Borrower continues payments                   |
    |  Principal balance decreases to zero           |
    |  Interest accrues until paid                   |
    +--------------------+----------------------------+
                         |
                         ▼
    STAGE 8: CLOSURE
    +-------------------------------------------------+
    |  Loan fully repaid                            |
    |  Loan account closed                          |
    |  Collateral released (secured)               |
    |  Money destroyed (principal portion)          |
    +-------------------------------------------------+
```

## 37. Real-World Example of Money Creation Through a Loan

Let's follow a complete example of how money is created when a bank makes a loan.

```
REAL-WORLD EXAMPLE

    +-------------------------------------------------+
    |  SCENARIO:                                       |
    |  Small business owner wants to expand           |
    |  Applies for $100,000 loan                      |
    +-------------------------------------------------+

    STEP 1: Application
    +-------------------------------------------------+
    |  Business owner submits application            |
    |  Business financials: Annual revenue $500,000  |
    |  Existing debt: $50,000                        |
    |  Credit score: 720 (Good)                      |
    |  Purpose: Purchase equipment                  |
    |  Repayment: 5 years                          |
    +-------------------------------------------------+

    STEP 2: Bank Evaluation
    +-------------------------------------------------+
    |  Credit check: Good history                    |
    |  Debt-to-income ratio: 30% (acceptable)       |
    |  Collateral: Equipment to be purchased         |
    |  Business viability: Strong                    |
    +-------------------------------------------------+

    STEP 3: Loan Approved
    +-------------------------------------------------+
    |  Amount: $100,000                              |
    |  Rate: 6% (fixed)                             |
    |  Term: 5 years (60 months)                    |
    |  Monthly EMI: $1,933                         |
    +-------------------------------------------------+

    STEP 4: Money Creation
    +-------------------------------------------------+
    |  Bank credits borrower's checking account     |
    |  New deposit of $100,000 created              |
    |  Bank creates new asset: Loan Receivable      |
    |  Bank creates new liability: Borrower Deposit |
    |  Money supply increases by $100,000           |
    +-------------------------------------------------+

    STEP 5: Borrower Uses the Money
    +-------------------------------------------------+
    |  Borrower buys $100,000 equipment             |
    |  Equipment supplier deposits check             |
    |  Money moves to supplier's bank               |
    |  Money remains in the system                  |
    +-------------------------------------------------+

    STEP 6: Repayment Process
    +-------------------------------------------------+
    |  Monthly payments of $1,933                   |
    |  First year: Mostly interest                  |
    |  Final year: Mostly principal                 |
    |  Over 5 years, $115,980 repaid                |
    |  Bank earns $15,980 in interest              |
    +-------------------------------------------------+

    STEP 7: Loan Fully Repaid
    +-------------------------------------------------+
    |  Principal ($100,000) destroyed               |
    |  Interest ($15,980) becomes bank income       |
    |  Money supply decreases by $100,000           |
    |  Bank earns profit from interest              |
    +-------------------------------------------------+
```

## 38. Common Misconceptions About Loans and Money Creation

```
COMMON MISCONCEPTIONS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   MISCONCEPTION 1: "Banks only lend money deposited by customers"          │
    │                                                                             │
    │   TRUTH: Banks create new money when they make loans. They do not         │
    │   simply lend existing deposits. The loan creates a new deposit.           │
    │                                                                             │
    │                                                                             │
    │   MISCONCEPTION 2: "Savers' money is used for loans"                      │
    │                                                                             │
    │   TRUTH: Deposits and loans are independent. Loans create deposits,        │
    │   not the reverse. Savings provide reserves, not lending funds.            │
    │                                                                             │
    │                                                                             │
    │   MISCONCEPTION 3: "Banks have a fixed pool of money to lend"             │
    │                                                                             │
    │   TRUTH: Banks can create unlimited money through lending, subject to     │
    │   reserve requirements, capital constraints, and borrower demand.         │
    │                                                                             │
    │                                                                             │
    │   MISCONCEPTION 4: "Money creation is printing physical currency"         │
    │                                                                             │
    │   TRUTH: Most money creation is digital. Banks create money by            │
    │   making electronic entries, not printing notes.                          │
    │                                                                             │
    │                                                                             │
    │   MISCONCEPTION 5: "Banks can create unlimited money"                     │
    │                                                                             │
    │   TRUTH: Banks are limited by reserve requirements, capital                │
    │   requirements, liquidity requirements, and the availability of            │
    │   creditworthy borrowers.                                                 │
    │                                                                             │
    │                                                                             │
    │   MISCONCEPTION 6: "Loan repayment creates new money"                     │
    │                                                                             │
    │   TRUTH: Loan repayment destroys money. The borrower's deposit is         │
    │   debited, and the loan asset is reduced. Money disappears.               │
    │                                                                             │
    │                                                                             │
    │   MISCONCEPTION 7: "Only central banks create money"                      │
    │                                                                             │
    │   TRUTH: Central banks create base money (currency, reserves).            │
    │   Commercial banks create broad money (deposits) through lending.         │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 39. Key Takeaways

```
KEY TAKEAWAYS

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   LOANS BASICS                                                             │
    │   ├── A loan is borrowed money with a promise to repay with interest      │
    │   ├── Loans enable purchases and investments beyond current resources     │
    │   ├── Different types serve different purposes (mortgage, auto, business) │
    │   └── Approval depends on the Five C's of Credit                         │
    │                                                                             │
    │   INTEREST AND REPAYMENT                                                   │
    │   ├── Interest is the cost of borrowing                                  │
    │   ├── Fixed rates stay constant, variable rates change                   │
    │   ├── EMIs are equal monthly installments covering principal and interest │
    │   └── Default occurs when repayment obligations are not met              │
    │                                                                             │
    │   MONEY CREATION THROUGH LENDING                                           │
    │   ├── Banks create new money when issuing loans                          │
    │   ├── No existing deposit is used—a new deposit is created               │
    │   ├── Fractional reserve banking enables money creation                  │
    │   └── Money multiplier multiplies base money into broad money            │
    │                                                                             │
    │   LIMITS AND CONTROLS                                                      │
    │   ├── Reserve requirements limit lending capacity                        │
    │   ├── Capital requirements constrain excessive lending                  │
    │   ├── Central banks set policy and supervise banks                       │
    │   └── Creditworthy borrowers are essential for lending                   │
    │                                                                             │
    │   IMPACTS AND RISKS                                                       │
    │   ├── Loans support economic growth through investment and consumption  │
    │   ├── Excessive lending can cause inflation and asset bubbles           │
    │   ├── Non-Performing Loans arise from borrower distress and poor          │
    │   │   underwriting                                                        │
    │   └── Banks manage risk through underwriting, diversification, reserves   │
    │                                                                             │
    │   MONEY DESTRUCTION                                                        │
    │   ├── Loan repayment destroys money                                     │
    │   ├── The borrower's deposit is debited                                 │
    │   ├── The loan asset is reduced                                          │
    │   └── Money supply decreases                                            │
    │                                                                             │
    │   THE COMPLETE CYCLE                                                      │
    │   ├── Application → Underwriting → Approval → Closing                    │
    │   ├── → Servicing → Monitoring → Repayment → Closure                     │
    │   └── Money created at origination, destroyed at repayment               │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

*This documentation belongs to https://github.com/InterCentury*