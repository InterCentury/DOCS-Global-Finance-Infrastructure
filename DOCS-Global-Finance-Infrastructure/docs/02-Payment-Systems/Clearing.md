
# DOCS-Global-Finance-Infrastructure/docs/02-Payment-Systems/Clearing.md

## Clearing

### 1. What is Clearing?
Clearing is the procedure by which financial institutions exchange payment instructions and calculate net obligations before the actual transfer of funds (settlement) occurs. It is the reconciliation of transactions between the payer's bank and the payee's bank.

### 2. Why Does Clearing Exist?
It exists to process the massive volume of daily transactions efficiently. Without clearing, banks would have to settle every single transaction individually in real-time, requiring immense liquidity and continuous manual or gross automated reconciliation.

### 3. What Problem Does Clearing Solve?
Clearing solves the "liquidity trap" and "transaction volume" problems. By batching and calculating obligations, it reduces the total amount of actual money that needs to move between institutions.

### 4. Where Does Clearing Fit in the Payment Lifecycle?
Clearing is the middle step in the payment lifecycle:
1. **Initiation & Authorization:** The payer requests the payment.
2. **Clearing:** Banks exchange data and calculate who owes whom.
3. **Settlement:** Actual funds are transferred between central bank accounts.

### 5. Clearing vs Settlement
```
┌────────────────────┬─────────────────────────────┬─────────────────────────────┐
│ Aspect             │ Clearing                    │ Settlement                  │
├────────────────────┼─────────────────────────────┼─────────────────────────────┤
│ Purpose            │ Calculate net obligations   │ Transfer actual funds       │
│ Timing             │ Middle stage (post-auth)    │ Final stage                 │
│ Action             │ Data exchange & matching    │ Liquidity movement          │
└────────────────────┴─────────────────────────────┴─────────────────────────────┘
```
### 6. Clearing vs Payment Processing
Payment processing handles the front-end capture, routing, and authorization of a transaction from a merchant or user interface. Clearing handles the back-end interbank reconciliation of that processed payment.

### 7. Clearing vs Authorization
Authorization is a real-time check to ensure the payer has sufficient funds and the account is valid. Clearing is the subsequent process where the authorized transaction's data is routed to the respective institutions to prepare for final settlement.

---

## Fundamentals

### 8. What Happens During Clearing?
Financial institutions transmit transaction batches to a central clearing facility. The facility validates the data, sorts transactions by receiving institution, calculates the net positions (credits vs. debits), and generates settlement instructions.

### 9. Who Participates in Clearing?
*   **Originating Depository Financial Institution (ODFI):** Submits payment instructions.
*   **Receiving Depository Financial Institution (RDFI):** Receives payment instructions.
*   **Clearing House / Operator:** The central entity processing the data.
*   **Central Bank:** (Often involved later for settlement).

### 10. What Is a Clearing House?
A central financial institution or network operator that facilitates the clearing process by acting as an intermediary, receiving files, sorting them, and computing net settlement totals.

### 11. What Is a Clearing Network?
The infrastructure (hardware, software, and communication protocols) connecting participating banks to the Clearing House. Examples include the ACH Network or CHIPS.

### 12. What Information Is Exchanged During Clearing?
Transactions contain routing numbers, account numbers, transaction amounts, transaction codes (credit/debit), settlement dates, and remitter/beneficiary metadata.

```text
       +-------------+
       | Originator  |
       +------+------+
              | Payment Request
              v
       +-------------+
       |   ODFI      |
       +------+------+
              | Batch File (ISO 20022/NACHA)
              v
       +-------------+
       | Clearing    | <--- Calculates Net Position
       | House       |
       +------+------+
              | Sorted Batch Data
              v
       +-------------+
       |   RDFI      |
       +------+------+
              | Account Credit/Debit
              v
       +-------------+
       |  Receiver   |
       +-------------+

```

---

## Clearing Lifecycle

### 13. Clearing Transaction Lifecycle

The lifecycle encompasses data ingestion, validation, matching, and position calculation.

### 14. Transaction Capture

The ODFI aggregates individual payment requests into a standard batch file format.

### 15. Transaction Validation

The clearing system checks the batch for structural integrity, correct formatting (e.g., correct ABA routing numbers), and cryptographic signatures.

### 16. Transaction Matching

In systems where both parties submit data (like securities), the clearing house matches the buy instruction with the sell instruction.

### 17. Transaction Verification

Ensuring the transaction adheres to network rules, limits, and compliance checks (e.g., AML/KYC metadata completeness).

### 18. Transaction Routing

The clearing house sorts the validated transactions and groups them by the destination RDFI.

### 19. Position Calculation

The system sums up all debits and credits for each participant to determine their gross position.

### 20. Net Obligation Calculation

The gross positions are netted against each other to determine the final, single settlement amount each bank owes or is owed.

```text
[Capture] -> [Validate] -> [Match/Verify] -> [Route] -> [Calculate Net] -> (To Settlement)

```

---

## Netting

### 21. What Is Netting?

Netting is the offsetting of payment obligations between two or more parties to arrive at a single net amount payable or receivable.

### 22. Why Is Netting Important?

It drastically reduces the amount of liquidity banks need to hold. If Bank A owes Bank B $100M, and Bank B owes Bank A $90M, netting means only $10M actually needs to move.

### 23. Gross Settlement vs Net Settlement
```
┌────────────────────┬──────────────────────────────┬──────────────────────────────┐
│ Feature            │ Gross Settlement (RTGS)      │ Net Settlement (ACH)         │
├────────────────────┼──────────────────────────────┼──────────────────────────────┤
│ Processing         │ Transaction by transaction   │ Batched at end of cycle      │
│ Liquidity Need     │ High (funds for every tx)    │ Low (only net difference)    │
│ Speed              │ Real-time                    │ Deferred (T+1, etc.)         │
└────────────────────┴──────────────────────────────┴──────────────────────────────┘
```
### 24. Bilateral Netting

Netting obligations directly between exactly two institutions.

### 25. Multilateral Netting

Netting obligations among three or more institutions through a central counterparty, resulting in one single net position per bank against the entire clearing house.

### 26. Net Settlement Example

```text
Without Netting (Gross):            With Multilateral Netting:
A pays B: $50                       Net Positions:
B pays C: $30                       A: - $50
C pays A: $40                       B: + $20 ($50 in - $30 out)
Total funds moved: $120             C: + $30 ($40 in - $30 out, wait math: C receives 30, pays 40 = -10)
                                    Corrected C: - $10, A: + $40 - $50 = - $10, B: + $50 - $30 = + $20
                                    Total funds moved: $20 (A pays $10, C pays $10 to B)

```

---

## Clearing Houses

### 27. What Is a Clearing House?

An intermediary entity that provides clearing and settlement services for financial transactions.

### 28. How Does a Clearing House Work?

It receives data files from members at designated cut-off times, runs netting algorithms, distributes sorted receiver files, and sends net settlement instructions to the central bank.

### 29. Why Are Clearing Houses Important?

They provide systemic stability, standardize communication, and act as a central hub, eliminating the need for complex, point-to-point connections between every bank in the world.

### 30. Clearing House Functions

* Rule enforcement and standardization.
* Data sorting and routing.
* Risk management and guarantee (in some markets).
* Dispute resolution.

### 31. Clearing House Risk Management

Clearing houses mitigate risk by requiring members to maintain collateral (clearing funds), enforcing strict admission criteria, and utilizing real-time monitoring of exposure.

---

## Banking Systems

### 32. Clearing in ACH Systems

ACH (Automated Clearing House) relies entirely on deferred net settlement. Batches are cleared multiple times a day (e.g., Same Day ACH) or overnight.

### 33. Clearing in Card Networks

Card networks (Visa/Mastercard) perform dual-message clearing. The authorization is message one. Clearing is message two, usually submitted in a daily batch by the acquiring bank to the network, which then routes it to the issuing bank.

### 34. Clearing in RTGS Systems

Real-Time Gross Settlement systems (like Fedwire) bypass traditional deferred clearing. The transaction is cleared and settled simultaneously in real-time.

### 35. Clearing in Interbank Transfers

Domestic interbank transfers rely on national clearing systems (e.g., BACS in the UK, STEP2 in Europe) to handle high-volume, low-value payments.

### 36. Clearing in Cross-Border Payments

Often relies on correspondent banking where clearing happens via bilateral accounts (Nostro/Vostro) or regional clearing hubs (like EBA CLEARING).

---

## Financial Markets

### 37. Clearing in Securities Markets

Involves matching buyers and sellers of equities/bonds and updating central securities depositories (CSDs).

### 38. Clearing in Stock Exchanges

A Central Counterparty (CCP) steps in between the buyer and seller. The CCP becomes the buyer to every seller and the seller to every buyer (Novation).

### 39. Clearing in Bond Markets

Similar to equities but often involves higher values and delivery-versus-payment (DvP) mechanisms to ensure the bond changes hands exactly when the money does.

### 40. Clearing in Derivatives Markets

Focuses heavily on margin calculation. The clearing house calculates daily mark-to-market variations and issues margin calls to cover potential future exposure.

### 41. Clearing in Futures Markets

Every contract is guaranteed by the clearing house, completely removing counterparty credit risk for individual traders.

---

## Risks

### 42. Clearing Risk

The general risk that a transaction fails to process successfully between the time of commitment and settlement.

### 43. Credit Risk During Clearing

The risk that a participating bank defaults and cannot fund its net debit position at the time of settlement.

### 44. Operational Risk During Clearing

The risk of system outages, data corruption, format errors, or cyberattacks disrupting the batch processing.

### 45. Settlement Risk

The risk (often called Herstatt Risk) that one party delivers the asset/currency, but the other party fails to deliver the counter-value.

### 46. Counterparty Risk

The risk that the other party in a bilateral agreement defaults. CCPs heavily mitigate this by standing in the middle.

---

## Technology

### 47. Clearing Infrastructure

Consists of secure file transfer protocols (SFTP, MQ), highly available mainframe or cloud computing clusters for position calculation, and secure network lines (e.g., SWIFTNet).

### 48. Clearing Messages

Historically proprietary (e.g., NACHA formats in the US). Modern systems are migrating globally to **ISO 20022**, an XML-based standard that allows rich data to travel with the clearing instruction.

### 49. Automated Clearing Systems

Systems that require zero manual intervention, relying on STP (Straight Through Processing) to validate, clear, and route based on predefined rules engines.

### 50. Real-Time Clearing

The evolution of clearing where netting is either continuous or bypassed entirely for 24/7/365 processing (e.g., The Clearing House's RTP network).

---

## Examples

### 51. ACH Clearing Example

An employer (Originator) submits a payroll file to Bank A (ODFI). Bank A sends the file to the Fed (Operator). The Fed sorts the file, calculates that Bank A owes Bank B $10,000, sends the transaction details to Bank B (RDFI), and settles the funds later.

### 52. Card Payment Clearing Example

A merchant batches all daily credit card swipes and sends them to their Acquirer. The Acquirer sends this to Visa. Visa calculates what the Acquirer is owed vs. what the Issuer must pay, netting out interchange fees.

### 53. Interbank Clearing Example

Bank X and Bank Y process thousands of checks and digital transfers. A central automated clearing house tallies them at 4:00 PM and settles the net difference via the Central Bank at 5:00 PM.

### 54. Securities Clearing Example

Trader A buys 100 shares of Apple. The trade goes to the DTCC (Clearing House), which novates the trade, updates ownership records, and calculates net cash obligations for the brokers.

### 55. End-to-End Clearing Flow Diagram

```text
+----------------+       +------------------+       +----------------+
|  Originator    |       |      ODFI        |       | Clearing House |
| (Submits File) | ----> | (Validates/Fwds) | ----> | (Nets & Sorts) |
+----------------+       +------------------+       +--------+-------+
                                                             |
                                                             | (Sends Net Settlement)
                                                             v
+----------------+       +------------------+       +----------------+
|   Receiver     |       |      RDFI        |       |  Central Bank  |
| (Gets Funds)   | <---- | (Posts to Acct)  | <---- | (Moves Money)  |
+----------------+       +------------------+       +----------------+

```

---

## Modern Clearing

### 56. Instant Payment Clearing

Systems like FedNow or SEPA Inst operate on a message-by-message basis, clearing and settling within seconds 24/7/365, bypassing traditional batch netting to provide immediate liquidity to the receiver.

### 57. Clearing in Digital Banking

Digital banks and FinTechs rely heavily on API-driven clearing integrations, often utilizing Banking-as-a-Service (BaaS) providers to connect to legacy clearing houses.

### 58. Future of Clearing Systems

The future points toward Distributed Ledger Technology (DLT) and blockchain, where atomic settlement (instant, simultaneous clearing and settlement on a shared ledger) could render traditional deferred netting obsolete.

---

## Summary

### 59. Key Concepts

* **Netting:** The core mathematical process of clearing.
* **ODFI/RDFI:** The sender and receiver institutional nodes.
* **CCP:** Central Counterparty, critical in securities for assuming risk.
* **ISO 20022:** The modern data standard for clearing messages.

### 60. Summary

Clearing is the indispensable nervous system of global finance. It transforms millions of disparate, high-volume transactions into organized, manageable net settlements. By separating the exchange of data from the movement of actual liquidity, clearing systems ensure that financial institutions can process modern commercial volumes efficiently, securely, and with minimized systemic risk.


