# Introduction to Payments

## Documentation Overview

A payment is the voluntary transfer of money, an equivalent, or other valuables from one party to another in exchange for goods, services, or to fulfill a legal obligation. In financial infrastructure, it is a set of messages and ledger updates that facilitate the transfer of value. This document provides a comprehensive introduction to payments: what they are, why they exist, how they work, who participates, and the systems that enable them.

## Documentation Objectives

```
DOCUMENTATION OBJECTIVES

    ┌─────────────────────────────────────────────────────────────────────────────┐
    │                                                                             │
    │   Understand the fundamental definition and purpose of payments             │
    │   Learn the participants and their roles in a payment transaction           │
    │   Study the complete payment lifecycle from initiation to finality          │
    │   Examine different types of payments and their characteristics             │
    │   Understand payment systems and their components                           │
    │   Learn about payment infrastructure and messaging standards                │
    │   Study the risks associated with payments and their mitigation             │
    │   Understand the regulatory framework governing payments                    │
    │   Learn about modern payment innovations (instant, open banking, APIs)      │
    │   Explore real-world payment examples                                       │
    │                                                                             │
    └─────────────────────────────────────────────────────────────────────────────┘
```

## 1. What Is a Payment

A payment is the voluntary transfer of money, an equivalent, or other valuables from one party to another in exchange for goods, services, or to fulfill a legal obligation. In financial infrastructure, it is a set of messages and ledger updates that facilitate the transfer of value.

How it works: A payment involves two key elements: the ```instruction``` to transfer value and the ```ledger update``` that records the transfer. The payer instructs their bank to debit their account and credit the payee's account. This instruction travels through payment networks, and ledgers are updated to reflect the new ownership of funds.

```
PAYMENT DEFINITION

                         +---------------------------+
                         |        PAYMENT            |
                         |  Voluntary transfer of    |
                         |  value between parties    |
                         +-------------+-------------+
                                       |
          +----------------------------+----------------------------+
          │                            │                            │
          ▼                            ▼                            ▼
+---------------------------+  +---------------------------+  +---------------------------+
|  KEY ELEMENTS             |  |  ESSENTIAL COMPONENTS     |  |  PURPOSE                  |
|  - Payer (sender)         |  |  - Instruction            |  |  - Exchange for goods     |
|  - Payee (receiver)       |  |  - Authorization          |  |  - Service payment        |
|  - Amount (value)         |  |  - Clearing               |  |  - Legal obligation       |
|  - Medium (cash, wire,    |  |  - Settlement             |  |  - Debt repayment         |
|    card, etc.)            |  |  - Finality               |  |  - Transfer of wealth     |
+---------------------------+  +---------------------------+  +---------------------------+
```

## 2. Why Do Payments Exist

Payments exist to facilitate economic trade. Without a standardized mechanism to transfer value, modern economies would rely on inefficient bartering systems. Payments abstract the concept of value exchange into universally accepted mediums.

How it works: In a barter economy, trade requires a ```double coincidence of wants```—each party must want exactly what the other offers. Payments solve this by introducing a universally accepted medium of exchange (money). Instead of trading goods directly, parties trade goods for money, and money for goods. This dramatically expands the possibilities for trade and economic activity.

## 3. What Problem Do Payment Systems Solve

Payment systems solve the problems of ```physical distance```, ```trust```, and ```scale```. They allow individuals and institutions to transfer value without physically exchanging raw assets (like gold or fiat currency notes) and without needing a direct trust relationship between the transacting parties.

The distance problem is solved by enabling electronic transfers across cities, countries, and continents. The trust problem is solved by using regulated financial institutions and secure messaging systems. The scale problem is solved by processing millions of transactions efficiently through automated systems.

## 4. What Makes a Payment Valid

A valid payment requires four essential conditions to be met.

```Consent``` means the payer explicitly authorizes the transfer. This can be through a signature, PIN, biometric, or digital authentication. Without consent, the payment is unauthorized and invalid.

```Availability of Funds``` means the payer has sufficient balance or credit to complete the transaction. If funds are insufficient, the payment must be declined or partially processed.

```Authentication``` means the identity of the payer and validity of the instruction are verified. This prevents fraud and ensures the instruction comes from the legitimate account holder.

```Non-repudiation``` means the transaction cannot be falsely denied by the payer post-execution. This provides proof that the payment was authorized and completed.

```
PAYMENT VALIDITY REQUIREMENTS

                         +---------------------------+
                         |  VALID PAYMENT            |
                         |  Four requirements        |
                         +-------------+-------------+
                                       |
          +----------------------------+----------------------------+
          │                            │                            │
          ▼                            ▼                            ▼
+---------------------------+  +---------------------------+  +---------------------------+
|  CONSENT                  |  |  AVAILABILITY OF FUNDS    |  |  AUTHENTICATION           |
|  - Explicit approval      |  |  - Sufficient balance     |  |  - Identity verified      |
|  - Signature/PIN          |  |  - Available credit       |  |  - Instruction valid      |
|  - Biometric              |  |  - No holds blocking      |  |  - Fraud screening        |
|  - Digital auth           |  |  - Within limits          |  |  - Multi-factor auth      |
+---------------------------+  +---------------------------+  +---------------------------+
          │                            │                            │
          +----------------------------+----------------------------+
                                       │
                                       ▼
                         +---------------------------+
                         |  NON-REPUDIATION          |
                         |  - Cannot be denied       |
                         |  - Audit trail exists     |
                         |  - Proof of execution     |
                         |  - Legal enforceability   |
                         +---------------------------+
```

## 5. What Is Value Transfer

Value transfer is the underlying mechanism of a payment. It is the ```accounting process``` where one ledger decreases its recorded value (debit) and another ledger increases its recorded value (credit) by the exact same amount.

How it works: When a payment occurs, the payer's account is debited (reduced) and the payee's account is credited (increased). This is ```double-entry bookkeeping```. The total amount of value in the system remains constant; it has simply been transferred from one owner to another. The payment message instructs these ledger updates.

## 6. Who Participates in a Payment

A standard digital payment involves at least four primary participants. More complex payments introduce additional intermediaries.

The ```payer``` (or originator) is the individual, business, or entity that initiates the payment and from whose account funds are debited.

The ```payer's financial institution``` (often called the Originating Depository Financial Institution or ODFI) is the bank that represents the payer and submits the payment instruction.

The ```payment network``` or ```intermediary``` is the infrastructure that routes the transaction between the payer's bank and the payee's bank. Examples include Visa, Mastercard, ACH, and SWIFT.

The ```payee's financial institution``` (often called the Receiving Depository Financial Institution or RDFI) is the bank that receives the payment instruction and credits the payee's account.

The ```payee``` (or beneficiary/receiver) is the entity designated to receive the funds.

```
PAYMENT PARTICIPANTS

       +---------+      +-------------+      +----------------+      +--------------+      +---------+
       |  Payer  | ---> | Payer's Bank| ---> | Payment Network| ---> | Payee's Bank | ---> |  Payee  |
       | (Buyer) |      |   (ODFI)    |      | (Intermediary) |      |    (RDFI)    |      | (Seller)|
       +---------+      +-------------+      +----------------+      +--------------+      +---------+
            │                │                    │                    │                      │
            │                │                    │                    │                      │
            ▼                ▼                    ▼                    ▼                      ▼
+---------------+  +----------------+      +----------------+     +---------------+   +---------------+
| Initiates     |  | Submits        |      | Routes         |     | Receives      |   | Receives      |
| payment       |  | instruction    |      | transaction    |     | instruction   |   | funds         |
| Authorizes    |  | Debits payer   |      | Processes data |     | Credits payee |   | Account       |
| transfer      |  | Sends to       |      | Applies rules  |     | Notifies      |   | credited      |
| Provides      |  | network        |      | Calculates net |     | payee         |   |               |
| account info  |  |                |      |                |     |               |   |               |
+---------------+  +----------------+      +----------------+     +---------------+   +---------------+
```

## 7. What Is a Payer

The payer (or originator) is the individual, business, or entity that initiates the payment and from whose account funds are debited.

The payer is the ```source of funds``` in any transaction. They provide the authorization for the payment and bear the responsibility for ensuring sufficient funds are available. The payer's identity, account information, and authorization are essential for the payment to be processed.

## 8. What Is a Payee

The payee (or beneficiary/receiver) is the entity designated to receive the funds. They are the ```final destination``` of the value transfer.

The payee provides their account information to receive the payment. They may be an individual receiving a salary, a business receiving payment for goods, or a government agency receiving taxes. The payee's bank credits their account when the payment is received.

## 9. What Is a Payment Service Provider (PSP)

A PSP is a third-party company that helps merchants accept payments. They exist to bridge the technical gap between a merchant's storefront and the complex banking networks.

How it works: A PSP aggregates payment methods (cards, bank transfers, digital wallets) into a single integration for merchants. They handle security, fraud detection, and settlement. They shield merchants from the complexity of direct banking relationships.

Examples of PSPs include Stripe, PayPal, Adyen, and Square.

## 10. What Is a Financial Institution

A financial institution (FI) is a regulated entity (usually a bank or credit union) that holds customer funds in accounts and participates directly in central clearing and settlement systems.

How it works: Financial institutions are the ```nodes``` of the payment system. They maintain customer accounts, process payment instructions, hold reserves at the central bank, and participate in clearing and settlement. They are regulated to ensure safety and soundness.

## 11. What Is a Payment Network

A payment network is the electronic infrastructure and set of rules that route transaction data and funds between financial institutions.

How it works: The network connects multiple financial institutions. It defines the ```rules``` for transaction processing, message formats, fees, and dispute resolution. It operates the technical infrastructure to route messages and (in some cases) settle funds.

Examples of payment networks include Visa, Mastercard, the ACH Network, and SWIFT.

## 12. How Does a Payment Work

A payment works by traversing a strict lifecycle of discrete steps, moving from an intention to pay, through risk checks, to interbank reconciliation, and finally, the irreversible transfer of central bank money.

How it works: The payment lifecycle is a sequence of phases that transform a payment instruction from initiation to final settlement. Each phase has specific functions, participants, and risks. Understanding the lifecycle is essential to understanding payments.

## 13. The Complete Payment Lifecycle

The complete payment lifecycle consists of five distinct phases that must occur for a payment to be successfully completed.

```Initiation``` is the creation and submission of a payment instruction by the payer. This is where the payment begins.

```Authorization``` is the real-time verification process. The payer's bank checks funds, validates the account, and approves the transaction.

```Clearing``` is the exchange of transaction details between banks to calculate net obligations. This is the data reconciliation phase.

```Settlement``` is the actual movement of funds to discharge obligations. This is where value actually transfers.

```Finality``` is the legal and operational moment when funds are unconditionally and irrevocably transferred.

```
PAYMENT LIFECYCLE

    INITIATION
       │
       │ Payer creates and submits payment instruction
       ▼
    AUTHORIZATION
       │
       │ Real-time verification of funds and identity
       ▼
    CLEARING
       │
       │ Banks exchange data, calculate net obligations
       ▼
    SETTLEMENT
       │
       │ Actual funds move between central bank accounts
       ▼
    FINALITY
       │
       │ Payment becomes irrevocable and unconditional
       ▼
    COMPLETE
```

## 14. Payment Initiation

```Initiation``` is the creation and submission of a payment instruction by the payer. This is the first step in the payment lifecycle.

How it works: A user swipes a card, clicks "pay" online, or submits a bulk file to a bank. This generates a structured data message containing all necessary payment details. The message includes the payer's account information, the payee's account information, the amount, and any additional instructions.

Examples of initiation include submitting a payroll batch file via a corporate banking portal, entering credit card details on an e-commerce website, or writing a physical check.

## 15. Payment Authorization

```Authorization``` is the real-time verification process. The payer's financial institution checks if the account is active, if funds are available, and if the transaction passes fraud checks. Funds are then placed on "hold."

How it works: The payment instruction is sent to the payer's bank. The bank verifies the account exists and is in good standing. It checks if the available balance (or credit limit) is sufficient. It runs fraud detection algorithms. If all checks pass, the bank ```authorizes``` the transaction and places a hold on the funds (reserving them for settlement). A confirmation (approval code) is sent back.

Examples include a card terminal saying "Approved" or an online payment receiving an authorization confirmation.

## 16. Payment Clearing

```Clearing``` is the exchange of transaction details between banks to calculate net obligations. This is the data reconciliation phase.

How it works: Banks send batches of authorized transactions to a clearing house. The clearing house validates, sorts, and calculates net positions. It determines exactly who owes whom and how much. No money actually moves during clearing; it is purely data processing.

Clearing occurs post-authorization and pre-settlement. It is the middle step of the payment lifecycle.

## 17. Payment Settlement

```Settlement``` is the actual movement of funds to discharge obligations. This is where value actually transfers.

How it works: Central banks adjust the master reserve accounts of participating commercial banks. If Bank A owes Bank B, the central bank debits Bank A's reserve account and credits Bank B's reserve account. This is the final transfer of funds. Settlement is the culmination of the payment process.

Settlement typically occurs in ```central bank money```, which is risk-free and final.

## 18. Payment Finality

```Finality``` is the legal and operational moment when funds are unconditionally and irrevocably transferred. Once final, a payment cannot be reversed except through a new, separate return transaction.

How it works: Finality occurs when settlement is complete and there is no further risk of failure or reversal. At this point, the payee has full legal claim to the funds. The payer cannot claw back the payment. Finality provides certainty to both parties.

Finality is the ultimate goal of any payment system. Systems that provide immediate finality (like RTGS) are considered safer than those with delayed finality (like ACH).

## 19. Cash Payments

```Cash``` payments are the physical transfer of fiat currency. They settle instantly upon physical handover.

How it works: The payer hands physical notes and coins to the payee. The payee accepts them and provides the goods or services. There is no intermediary, no clearing, and no settlement delay. The transaction is complete and final at the moment of handover.

Cash fits at the base retail level of the economy. It is anonymous, immediate, and requires no infrastructure. However, it is limited by physical distance and security risks.

## 20. Check Payments

```Check``` payments are paper-based instructions directing a bank to pay a specific amount. They exist as a legacy deferred-payment mechanism.

How it works: The payer writes a check (a paper instruction) and gives it to the payee. The payee deposits the check at their bank. The payee's bank sends the check to the payer's bank for collection. The payer's bank verifies the signature and funds, then debits the payer's account and credits the payee's bank. The payee's bank credits the payee's account.

Check processing relies heavily on physical or image-based clearing (Check 21 in the US). Checks are slow, expensive, and declining in use.

## 21. Bank Transfers

```Bank transfers``` are direct electronic transfers of funds from one account to another. They include wire transfers and ACH transfers.

How it works: The payer instructs their bank to transfer funds to the payee's bank. The instruction is sent electronically through a payment network (ACH, Fedwire, SWIFT). The payer's bank debits the payer's account and sends a payment message. The payee's bank receives the message and credits the payee's account.

Bank transfers are secure, efficient, and widely used. They form the backbone of wholesale and consumer payments.

## 22. Card Payments

```Card payments``` are payments facilitated by card networks using plastic cards or digital equivalents. They involve complex dual-message systems (Authorization then Clearing/Settlement).

How it works: The payer presents their card (physical or digital). The merchant sends an authorization request to their acquirer. The acquirer routes it through the card network (Visa, Mastercard) to the issuer (payer's bank). The issuer authorizes and holds funds. Later, the merchant submits a clearing file. The network processes clearing and settlement. Funds move from the issuer to the acquirer, and the merchant is paid.

Card payments are the dominant retail payment method globally.

## 23. Mobile Payments

```Mobile payments``` are payments initiated via mobile devices, often utilizing NFC (Near Field Communication) or QR codes. They are heavily integrated with digital wallets.

How it works: The payer uses a mobile app to initiate a payment. The app may use NFC to communicate with a payment terminal (tap-to-pay) or generate a QR code for scanning. The payment is processed through a card network or bank transfer system. The payer authenticates using a PIN, fingerprint, or facial recognition.

Mobile payments are growing rapidly, especially in emerging markets.

## 24. Digital Wallet Payments

```Digital wallet``` payments are software-based systems that securely store users' payment information and passwords for numerous payment methods and websites.

How it works: The payer stores their payment credentials (credit cards, bank accounts) in a digital wallet app (Apple Pay, Google Wallet). When making a payment, the wallet generates a token (not the actual card number) to protect the payer's information. The token is transmitted for authorization. The wallet provider manages the security and tokenization.

Digital wallets simplify payments and enhance security through tokenization.

## 25. Real-Time Payments

```Real-time payments``` are systems where the initiation, clearing, and settlement occur continuously, 24/7/365, within seconds.

How it works: The payer initiates a payment. The payment message is sent to the payee's bank in real time. Funds are immediately verified and transferred. The payee receives confirmation and access to funds within seconds. Settlement occurs immediately through central bank accounts.

Examples include RTP (The Clearing House) and FedNow in the US. Real-time payments provide immediate finality and 24/7 availability.

## 26. Cross-Border Payments

```Cross-border payments``` are transactions where the payee and payer are in different countries, requiring currency conversion and correspondent banking networks.

How it works: The payer's bank sends a payment instruction through SWIFT to a correspondent bank in the payee's country. The correspondent bank converts currency (if needed) and credits the payee's bank. The payee's bank credits the payee's account. Cross-border payments are slower and more expensive than domestic payments.

SWIFT is the primary messaging network for cross-border payments. CLS (Continuous Linked Settlement) reduces FX settlement risk.

```
PAYMENT TYPES COMPARISON

                         +---------------------------+
                         |  PAYMENT TYPE COMPARISON  |
                         +-------------+-------------+
                                       |
          +----------------------------+----------------------------+
          │                            │                            │
          ▼                            ▼                            ▼
+---------------------------+---------------------------+---------------------------+
|  PAYMENT TYPE             |  SPEED                    |  REVERSIBILITY            |
+---------------------------+---------------------------+---------------------------+
|  Wire Transfer            |  Hours                    |  Irrevocable              |
|  ACH                      |  1-3 Days                 |  Reversible               |
|  Card Payment             |  Seconds (Auth)           |  Chargebackable           |
|  Real-Time (RTP)          |  Seconds (Settle)         |  Irrevocable              |
|  Cash                     |  Immediate                |  Irrevocable              |
|  Check                    |  Days                     |  Reversible               |
+---------------------------+---------------------------+---------------------------+
```

## 27. What Is a Payment System

A payment system is an operational configuration of institutions, rules, procedures, standards, and technical infrastructure designed to facilitate the transfer of value.

How it works: A payment system brings together all the necessary components for payments to occur. It includes the ```legal framework``` (laws and regulations), the ```clearing infrastructure``` (data processing), the ```settlement assets``` (central bank money), the ```operating rules``` (network rules), and the ```participants``` (banks, PSPs, customers).

Payment systems can be retail (high-volume, low-value) or wholesale (low-volume, high-value). They can be domestic (single currency, single jurisdiction) or international (multiple currencies, multiple jurisdictions).

## 28. Components of a Payment System

A complete payment system requires several essential components working together.

The ```legal framework``` provides the legal basis for payment obligations, settlement finality, and enforcement.

The ```clearing infrastructure``` processes transaction data, validates entries, and calculates net obligations.

The ```settlement assets``` are the ultimate means of payment, typically central bank reserves.

The ```operating rules``` define participant obligations, transaction formats, and dispute resolution.

The ```participants``` include banks, payment service providers, and customers.

## 29. Retail Payment Systems

```Retail payment systems``` are high-volume, low-value systems designed for consumers and businesses.

How it works: Retail systems prioritize throughput and cost-efficiency. They handle millions of transactions daily, each of relatively small value. The focus is on low cost per transaction, high availability, and ease of use. Settlement may be deferred to reduce costs.

Examples include ACH (US), BACS (UK), and card networks (Visa, Mastercard).

## 30. Wholesale Payment Systems

```Wholesale payment systems``` are low-volume, extremely high-value systems used primarily between banks and financial markets.

How it works: Wholesale systems prioritize speed, security, and immediate finality. They handle large-value transactions (often millions or billions) between financial institutions. Settlement is typically in real time (RTGS) to eliminate settlement risk.

Examples include Fedwire (US), TARGET2 (EU), and CHAPS (UK).

## 31. Domestic Payment Systems

```Domestic payment systems``` operate within a single jurisdiction and utilize a single currency under one legal framework.

How it works: Domestic systems process payments where both the payer and payee are in the same country. They use the national currency and are governed by national laws and regulations. Settlement occurs through the national central bank.

Domestic systems are typically faster and cheaper than international systems.

## 32. International Payment Systems

```International payment systems``` are networks designed to pass messages and settle funds across borders, involving multiple currencies and regulatory environments.

How it works: International systems connect banks across countries. They handle currency conversion, correspondent banking relationships, and compliance with multiple regulatory regimes. They are slower and more expensive than domestic systems.

Examples include SWIFT (messaging) and CLS (settlement).

## 33. What Is Payment Infrastructure

Payment infrastructure is the physical hardware, network lines, data centers, and software protocols that physically transmit financial data between institutions.

How it works: The infrastructure includes the ```hardware``` (servers, routers, network lines), the ```software``` (messaging systems, clearing engines), and the ```protocols``` (communication standards). It must be secure, reliable, and highly available.

Payment infrastructure is the "plumbing" of the financial system. It operates behind the scenes to enable payments.

## 34. Payment Messages

Payment messages are the structured data formats used to transmit payment information. Historically proprietary, the industry is converging on ```ISO 20022```, a rich XML-based standard.

How it works: A payment message contains all the information needed to process a payment: sender, receiver, amount, currency, value date, and additional remittance information. The message format must be understood by both the sending and receiving systems.

ISO 20022 provides a common language for payment messages across different systems and countries. It supports richer data than legacy formats.

## 35. Payment Instructions

Payment instructions are the specific payload within a payment message detailing the exact debit account, credit account, amount, and value date.

How it works: The instruction is the "action" part of the payment message. It tells the receiving system exactly what to do: which account to debit, which to credit, how much, and when. The instruction must be unambiguous and complete.

## 36. Payment Routing

Payment routing is the logic used to determine the optimal path for a payment instruction to reach its destination.

How it works: Routing relies on identifiers such as routing numbers (ABA in US), BICs (Bank Identifier Codes), or IBANs (International Bank Account Number). The routing system determines the best path based on network topology, cost, speed, and availability.

## 37. Payment Processing

Payment processing is the computational execution of evaluating, authorizing, and updating ledger states based on payment messages.

How it works: Processing involves receiving the payment message, validating it, applying business rules, executing the transaction (debit/credit), and updating ledgers. Processing may be done in real-time (for card authorizations) or batch (for ACH).

## 38. Payment Networks

Payment networks are the overarching technical and legal entities (like ACH or Visa) that govern the infrastructure and define the rules of engagement.

How it works: The network establishes the ```rules``` for participation, the ```standards``` for messages, the ```fee structure```, and the ```dispute resolution``` process. It operates the technical infrastructure and ensures all participants follow the rules.

## 39. How Does Money Move Between Accounts

Money moves via ```double-entry bookkeeping```. A bank debits the sender's account liability and credits the receiver's account liability.

How it works: When a payment occurs, the payer's bank reduces the payer's account balance (debit) and increases the payee's account balance (credit). This is a purely accounting exercise—no physical money moves. The bank's balance sheet remains balanced: assets equal liabilities.

## 40. How Do Banks Transfer Money

Banks transfer money between themselves using reserves held at a central bank. If Bank A owes Bank B, the central bank debits Bank A's reserve account and credits Bank B's reserve account.

How it works: Commercial banks hold reserve accounts at the central bank. These accounts are used for interbank settlement. When a payment is made between customers of different banks, the banks' reserve accounts are adjusted. This is the ```ultimate settlement``` of the payment.

## 41. Why Doesn't Money Physically Move

Physical movement is slow, expensive, and dangerous. Because modern fiat money is primarily digital debt (bank liabilities), moving money simply requires secure, authenticated message passing to update disparate database ledgers.

How it works: Physical currency is only a small fraction of the total money supply. The vast majority of money exists only as digital records (bank liabilities). Moving money means updating these records, not moving physical objects. This is faster, cheaper, and more secure.

## 42. Account-Based vs Token-Based Payments

```Account-based``` payments require identity verification. To transfer value, the system must verify who you are to authorize a ledger update.

In account-based systems, the ```identity of the payer``` is the key to authorization. The system confirms you are the account holder and that you have authority to transfer funds. Examples include bank transfers, ACH, and card payments.

```Token-based``` payments verify the validity of the token. Whoever holds the token holds the value.

In token-based systems, the ```token itself``` is the key to value. The system does not need to know who holds the token, only that the token is valid. Examples include physical cash (the paper note is the token) and cryptocurrencies (the private key is the token).

```
ACCOUNT-BASED VS TOKEN-BASED

                         +---------------------------+
                         |  ACCOUNT-BASED vs        |
                         |  TOKEN-BASED PAYMENTS    |
                         +-------------+-------------+
                                       |
          +----------------------------+----------------------------+
          │                                                         │
          ▼                                                         ▼
+---------------------------+                            +---------------------------+
|  ACCOUNT-BASED           |                            |  TOKEN-BASED             |
|  (Identity-based)        |                            |  (Token-based)           |
|                           |                            |                           |
|  - Identity is key      |                            |  - Token is key          |
|  - Verify who you are   |                            |  - Verify token validity  |
|  - Authorization based  |                            |  - Whoever holds token   |
|    on identity         |                            |    holds value          |
|  - Examples: Bank       |                            |  - Examples: Cash,      |
|    transfers, ACH,     |                            |    cryptocurrency       |
|    card payments       |                            |                           |
+---------------------------+                            +---------------------------+
```

## 43. Payment Risk

Payment risk is the broad probability that a payment transaction will fail, be delayed, or result in financial loss to a participant.

How it works: Payment risk includes multiple types of risk: fraud, operational failure, counterparty default, and settlement failure. Payment systems are designed to minimize these risks through security, rules, and risk management procedures.

## 44. Fraud Risk

Fraud risk is the risk of unauthorized access or manipulation, resulting in stolen funds.

How it works: Fraud can occur through stolen credentials, phishing, insider threats, or system breaches. Mitigation includes ```Multi-Factor Authentication (MFA)```, ```tokenization```, ```anomaly detection```, and ```transaction monitoring```.

Payment systems must continuously evolve to address new fraud vectors.

## 45. Operational Risk

Operational risk is the risk of loss resulting from inadequate or failed internal processes, human error, or system outages.

How it works: A data center going offline, a software bug, or a human data entry error can disrupt payment processing. Mitigation includes ```redundant systems```, ```disaster recovery```, ```automated validation```, and ```rigorous testing```.

## 46. Settlement Risk

Settlement risk is the risk that one party in a transaction delivers the asset or currency, but the other party fails to deliver the counter-value. This is also known as ```Herstatt risk``` in foreign exchange.

How it works: In cross-currency transactions, the time zones create a gap between deliveries. If one bank delivers its currency but the other bank fails to deliver the counterparty currency, the delivering bank suffers a loss. Settlement risk is the primary risk addressed by RTGS systems and payment-versus-payment (PvP) mechanisms.

## 47. Counterparty Risk

Counterparty risk is the risk that the other party to an agreement will default before the final settlement of the transaction.

How it works: If a bank fails between trade execution and settlement, the counterparty may not receive their funds. This risk is mitigated by ```clearing houses``` acting as Central Counterparties (CCPs). The CCP stands between the two parties, guaranteeing the transaction.

## 48. Why Are Payment Systems Regulated

Payment systems are regulated to ensure ```systemic stability```, prevent financial crises, protect consumer funds, and prevent the financial system from being used for illicit activities.

How it works: Regulation establishes the rules, oversight, and enforcement mechanisms that ensure payment systems operate safely and fairly. Regulators monitor compliance, enforce standards, and intervene when risks arise.

## 49. AML in Payments

```Anti-Money Laundering (AML)``` involves laws and procedures to prevent criminals from disguising illegally obtained funds as legitimate income.

How it works: AML requires transaction monitoring (watching for suspicious patterns), reporting of suspicious activity (SARs), and customer due diligence. Payment systems must have AML controls to prevent their use for money laundering.

## 50. KYC in Payments

```Know Your Customer (KYC)``` is the mandatory process of identifying and verifying the identity of clients before allowing them access to payment networks.

How it works: KYC requires collecting and verifying customer information: name, address, date of birth, and identification documents. This ensures the payment system is not used for illicit purposes and helps prevent fraud.

## 51. Payment Compliance

Payment compliance is the ongoing adherence to regional rules (like PSD2 in Europe, or CFPB regulations in the US), sanctions lists (OFAC), and network operating rules.

How it works: Payment systems must monitor compliance requirements and ensure they are met. This includes screening against sanctions lists, following fair practices, and maintaining audit trails. Non-compliance can result in fines, penalties, or loss of network access.

## 52. Instant Payments

```Instant payments``` are account-to-account systems that provide immediate, irrevocable availability of funds to the payee, available 24/7.

How it works: Instant payments use ISO 20022 messaging and settle continuously. The payer initiates the payment. Funds are immediately verified and transferred. The payee receives confirmation within seconds. Settlement is immediate through central bank accounts.

Examples include RTP (The Clearing House), FedNow (US Federal Reserve), and SEPA Instant (Europe).

## 53. Open Banking Payments

```Open Banking``` is a framework where banks allow third-party providers (TPPs) secure access to consumer banking data via APIs to initiate payments directly from bank accounts, bypassing card networks.

How it works: The consumer authorizes a TPP to access their bank account. The TPP uses APIs to initiate a payment from the consumer's account to the merchant's account. The payment is processed as a bank transfer, avoiding card network fees. Authorization is done through secure authentication.

Open banking is regulated by PSD2 in Europe and similar frameworks elsewhere.

## 54. API-Based Payments

```API-based payments``` represent the shift from batch-file processing (like SFTP) to RESTful APIs, allowing software applications to embed payment initiation directly into their workflows seamlessly.

How it works: Instead of submitting batch files at designated times, applications can initiate payments in real time through APIs. The API handles authentication, authorization, and processing. This enables integration with accounting systems, e-commerce platforms, and mobile apps.

## 55. Digital Wallets

```Digital wallets``` are applications holding digitized versions of payment methods. They utilize network tokenization to process payments without exposing the underlying Primary Account Number (PAN).

How it works: The wallet stores payment credentials securely. When a payment is made, the wallet generates a ```token``` (a temporary, one-time-use identifier) instead of transmitting the actual card number. The token is processed through the payment network. This reduces fraud risk because the actual card number is never transmitted.

## 56. CBDCs and Future Payments

```Central Bank Digital Currencies (CBDCs)``` are digital forms of a country's fiat currency. They represent direct central bank liability to the citizen, potentially removing commercial banks from the settlement layer.

How it works: A CBDC is issued by the central bank and is a liability of the central bank (like physical cash, but digital). It can be used for peer-to-peer payments, retail purchases, and wholesale settlement. CBDCs could provide greater efficiency, financial inclusion, and programmability.

## 57. Cash Payment Example

Alice buys a $5 coffee from Bob. Alice hands Bob a $5 bill. The transaction is instantly initiated, cleared, and settled physically. ```Finality is immediate```.

No intermediaries, no clearing, no settlement delay. The transaction is complete at the moment of handover.

## 58. Card Payment Example

Alice buys a $50 book on Amazon.

Step 1: Alice enters Visa card details. Step 2: Amazon's PSP (Stripe) sends an authorization request to Visa. Step 3: Visa routes the request to Alice's bank (Issuer). Step 4: The Issuer checks funds, holds $50, and returns "Approved." Step 5: Amazon ships the book. Step 6: Overnight, Amazon's bank (Acquirer) requests the actual funds via clearing.

The authorization holds the funds. Clearing and settlement happen later.

## 59. Bank Transfer Example

Alice (Chase) pays her $1,000 rent to her landlord (Wells Fargo) via ACH.

Step 1: Chase batches the $1,000 instruction. Step 2: Chase sends the file to the Fed ACH Operator. Step 3: The Fed nets all daily Chase/WF transactions. Step 4: The Fed credits WF's reserve account and debits Chase's. Step 5: WF credits the landlord's account the next morning.

The payment is cleared and settled overnight.

## 60. Cross-Border Payment Example

Alice in the US wires $10,000 to Bob in the UK.

Step 1: Alice's US bank sends a SWIFT MT103 message to a UK correspondent bank. Step 2: US bank debits Alice $10,000. Step 3: US bank credits the UK correspondent's Nostro account in NY. Step 4: UK correspondent debits its Nostro and credits Bob's bank via UK CHAPS. Step 5: Bob's bank credits Bob in GBP.

Cross-border payments involve multiple banks, currencies, and systems.

## 61. Key Payment Concepts

```Ledgers``` are the foundation of payments. Payments are simply coordinated updates to ledgers. Understanding ledgers is essential to understanding payments.

The ```separation of phases``` is critical. Authorization (permission), Clearing (calculation), and Settlement (money movement) are distinct phases with different risks and timeframes.

```Risk``` is the primary driver of payment system design. Systems are fundamentally designed to eliminate counterparty and settlement risks.

## 62. Summary

Payments form the critical plumbing of the global economy. Understanding payments requires shifting focus away from physical money and toward secure messaging, ledger management, and risk mitigation.

From simple cash handovers to multi-leg cross-border SWIFT transfers, all payment systems attempt to achieve the same goal: ```moving value securely, quickly, and with absolute finality```.

```
SUMMARY

    +-------------------------------------------------+
    |  WHAT IS A PAYMENT?                             |
    |  Voluntary transfer of value between parties   |
    |  in exchange for goods, services, or to       |
    |  fulfill a legal obligation                   |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  WHY PAYMENTS EXIST?                           |
    |  Facilitate economic trade                     |
    |  Abstract value exchange into universal       |
    |  medium                                       |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  PAYMENT LIFECYCLE                             |
    |  Initiation → Authorization → Clearing →      |
    |  Settlement → Finality                        |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  KEY PARTICIPANTS                              |
    |  Payer, Payer's Bank (ODFI), Payment Network,  |
    |  Payee's Bank (RDFI), Payee                   |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  PAYMENT TYPES                                 |
    |  Cash, Checks, Bank Transfers, Cards,         |
    |  Mobile, Digital Wallets, Real-Time,          |
    |  Cross-Border                                |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  PAYMENT SYSTEMS                               |
    |  Retail (high-volume, low-value)              |
    |  Wholesale (low-volume, high-value)           |
    |  Domestic (single currency)                   |
    |  International (multiple currencies)          |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  RISKS                                         |
    |  Fraud, Operational, Settlement (Herstatt),   |
    |  Counterparty                                 |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  REGULATION                                    |
    |  AML, KYC, Compliance, Consumer protection    |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  MODERN PAYMENTS                               |
    |  Instant Payments, Open Banking, APIs,        |
    |  Digital Wallets, CBDCs                       |
    +-------------------------------------------------+

    +-------------------------------------------------+
    |  KEY TAKEAWAY                                  |
    |  Payments are secure messages that update     |
    |  ledgers. They move value, not physical       |
    |  money. The goal is speed, security, and      |
    |  finality.                                   |
    +-------------------------------------------------+
```

*This documentation belongs to https://github.com/InterCentury*