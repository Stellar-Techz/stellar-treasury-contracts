AI Treasury Agent

An AI-powered programmable treasury built on Stellar, where AI analyzes treasury activity and Soroban smart contracts enforce secure spending rules and authorized on-chain actions.

🚀 Overview

Managing a blockchain treasury can be difficult.

Businesses, startups, DAOs, organizations, and Web3 projects need to constantly monitor:

Wallet balances
Incoming and outgoing payments
Treasury reserves
Spending patterns
Suspicious transactions
Recurring payments
Operational expenses

Most of this is still done manually.

AI Treasury Agent provides an intelligent treasury assistant that monitors on-chain activity, analyzes financial behavior, detects unusual activity, recommends actions, and can execute authorized treasury operations.

The key principle is:

AI provides the intelligence.

Soroban smart contracts enforce the rules.

Stellar provides the fast and efficient settlement layer.

🎯 Problem

Managing a treasury manually creates several problems.

1. Constant monitoring

Treasury owners have to repeatedly check their wallets and transactions.

2. Difficult transaction analysis

A treasury can have many transactions, making it difficult to understand where money is going.

3. Unusual activity can be missed

A large or unexpected payment may not be noticed quickly.

4. Manual treasury operations

Recurring payments and reserve management require someone to manually perform transactions.

5. AI needs controlled access

Giving an AI unrestricted access to treasury funds creates a serious security risk.

💡 Solution

AI Treasury Agent combines:

AI + Soroban Smart Contracts + Stellar

to create a programmable treasury.

The AI can:

Monitor treasury balances
Analyze transactions
Detect unusual activity
Generate treasury reports
Recommend actions
Evaluate treasury rules
Prepare transactions
Execute authorized low-risk operations

However, the AI does not have unlimited access to the treasury.

The Soroban smart contract enforces:

Spending limits
Daily limits
Authorized agents
Approved recipients
Allowed assets
Treasury rules
Emergency pause
Owner permissions
🧠 How It Works
                    USER
                     │
                     ▼
                Web Dashboard
                     │
          ┌──────────┴──────────┐
          │                     │
          ▼                     ▼
       AI Agent              Stellar Wallet
          │                     │
          │                     │
          ▼                     │
   Analyze & Decide              │
          │                     │
          ▼                     │
    Create Action                │
          │                     │
          └──────────┬──────────┘
                     ▼
             Soroban Contract
                     │
          ┌──────────┼──────────┐
          │          │          │
          ▼          ▼          ▼
       Limits     Permissions  Rules
          │          │          │
          └──────────┼──────────┘
                     ▼
                  Stellar
                     │
                     ▼
                Transaction
🔐 Core Security Model

The most important principle is:

The AI never receives unrestricted control over the treasury.

The treasury owner defines what the AI is allowed to do.

For example:

Agent Permissions

Maximum transaction: $500

Daily spending limit: $2,000

Allowed asset: USDC

Approved recipient:
GABC...

Agent:
GXYZ...

If the AI attempts to transfer more than the configured limit, the Soroban contract rejects the operation.

AI requests $10,000
        │
        ▼
Soroban Contract
        │
        ▼
Maximum = $500
        │
        ▼
       ❌
     REJECT

The smart contract therefore becomes the security boundary between the AI and the treasury.

⭐ Core Features
1. Stellar Wallet Connection

Users connect a Stellar-compatible wallet.

The application can display:

XLM balance
USDC balance
Other supported Stellar assets
Treasury value
Transaction history
Treasury activity
2. Programmable Treasury Vault

Users can deposit supported Stellar assets into the treasury contract.

For example:

Treasury

XLM      $2,000
USDC    $10,000
EURC     $5,000
----------------
Total   $17,000

The Soroban contract manages the treasury according to the owner's configured policies.

3. AI Treasury Agent

The AI analyzes treasury activity.

Users can ask:

"How is my treasury doing?"

"Show me unusual transactions."

"How much did we spend this month?"

"What are our biggest expenses?"

"What should I do with my excess funds?"

The AI analyzes available treasury data and responds with useful insights.

4. Transaction Monitoring

The backend monitors Stellar transactions associated with the treasury.

For example:

Incoming
+ 2,000 USDC

Outgoing
- 400 USDC

Outgoing
- 7,500 USDC

The AI can identify that the 7,500 USDC payment is significantly larger than normal treasury activity.

5. AI Anomaly Detection

The AI analyzes transaction patterns.

For example:

Normal transactions:

100 USDC
250 USDC
400 USDC
300 USDC

New transaction:

8,000 USDC

The agent can report:

⚠️ An unusual 8,000 USDC transaction was detected. This is significantly larger than your recent transaction pattern.

The system does not automatically claim that the transaction is fraudulent.

It simply flags the activity for review.

6. Treasury Rules

Treasury owners can define programmable rules.

Example:

IF

Treasury balance < 2,000 USDC

THEN

Notify treasury owner

Another:

IF

Transaction > 1,000 USDC

THEN

Require manual approval

Another:

EVERY FRIDAY

Transfer 100 USDC

TO

Approved reserve wallet

These rules can be enforced by the Soroban contract.

🤖 AI Agent Execution Modes

The application can support three levels of automation.

Mode 1 — Recommend

The AI only recommends an action.

AI
 ↓
Recommendation
 ↓
User decides

Example:

"I recommend moving 500 USDC to your reserve wallet."

Mode 2 — Approval Required

The AI prepares the transaction.

AI
 ↓
Prepare transaction
 ↓
User approves
 ↓
Soroban Contract
 ↓
Stellar

This is useful for larger or sensitive transactions.

Mode 3 — Automated

The AI can execute predefined low-risk actions.

AI
 ↓
Check rule
 ↓
Check permissions
 ↓
Check limits
 ↓
Soroban Contract
 ↓
Execute

Example:

Automatically transfer 100 USDC to the approved reserve wallet every Friday.

🛡️ Soroban Smart Contract Security

The Soroban treasury contract should enforce several controls.

Agent Authorization

Only an authorized AI agent can request automated actions.

Transaction Limits

The maximum amount that can be transferred in one transaction.

Daily Limits

The maximum amount the agent can move during a defined period.

Asset Allowlist

Only supported Stellar assets can be transferred.

Recipient Allowlist

The AI can only send funds to approved addresses.

Emergency Pause

The treasury owner can stop automated operations.

Owner Controls

Only authorized users can change critical treasury settings.

🧩 Example

Imagine a company has:

20,000 USDC

inside its Stellar treasury.

The owner configures:

Transaction limit: 500 USDC

Daily limit: 2,000 USDC

Approved reserve wallet:
GABC...

Authorized AI agent:
GXYZ...

The AI notices that the treasury has excess operating funds.

It recommends:

"Move 500 USDC to the reserve wallet."

The Soroban contract checks:

Agent authorized?       ✅

Amount <= 500 USDC?     ✅

Recipient approved?     ✅

Daily limit available?  ✅

Asset allowed?          ✅

The transaction is then executed on Stellar.

🔥 Why Soroban Is Important

The smart contract is not just there to make the project "Web3."

It provides the actual treasury security model.

Instead of trusting the AI:

AI → Wallet → Money

we use:

AI
 │
 ▼
Soroban Contract
 │
 ├── Is the agent authorized?
 ├── Is the amount allowed?
 ├── Is the recipient approved?
 ├── Is the asset allowed?
 └── Is the daily limit available?
 │
 ▼
Stellar

This means the AI operates within rules enforced on-chain.

🏗️ System Architecture
┌──────────────────────────────────────┐
│             Frontend                 │
│              Next.js                 │
└──────────────────┬───────────────────┘
                   │
                   ▼
┌──────────────────────────────────────┐
│             Backend                  │
│              NestJS                  │
├──────────────────────────────────────┤
│                                      │
│  AI Agent Service                    │
│  Treasury Service                    │
│  Transaction Monitor                 │
│  Rule Engine                         │
│  Analytics Service                   │
│                                      │
└───────────────┬──────────────────────┘
                │
       ┌────────┴────────┐
       │                 │
       ▼                 ▼
 PostgreSQL           AI Provider
       │
       │
       ▼
┌──────────────────────────────────────┐
│              Stellar                 │
│                                      │
│          Soroban Contract             │
│                                      │
│        TreasuryVault Contract         │
└──────────────────────────────────────┘
🛠️ Technology Stack
Frontend
Next.js
TypeScript
Tailwind CSS
Stellar Wallet Kit
Stellar SDK
Backend
NestJS
TypeScript
Prisma
PostgreSQL
Redis
AI
LLM API
AI Agent Service
Rule Evaluation Engine
Blockchain
Stellar
Soroban
Rust
Stellar SDK
Smart Contract
TreasuryVault

Written in:

Rust

and deployed to:

Soroban
📂 Project Structure
ai-treasury-agent-stellar/
│
├── apps/
│   │
│   ├── web/
│   │   ├── app/
│   │   │   ├── dashboard/
│   │   │   ├── treasury/
│   │   │   ├── transactions/
│   │   │   ├── rules/
│   │   │   ├── agent/
│   │   │   └── settings/
│   │   │
│   │   ├── components/
│   │   │   ├── treasury/
│   │   │   ├── agent/
│   │   │   ├── transactions/
│   │   │   └── wallet/
│   │   │
│   │   ├── lib/
│   │   │   ├── stellar/
│   │   │   └── api/
│   │   │
│   │   └── package.json
│   │
│   └── api/
│       ├── src/
│       │   │
│       │   ├── auth/
│       │   │
│       │   ├── users/
│       │   │
│       │   ├── treasury/
│       │   │
│       │   ├── transactions/
│       │   │
│       │   ├── agent/
│       │   │   ├── agent.service.ts
│       │   │   ├── agent.controller.ts
│       │   │   ├── agent.module.ts
│       │   │   └── prompts/
│       │   │
│       │   ├── rules/
│       │   │   ├── rules.service.ts
│       │   │   ├── rules.controller.ts
│       │   │   └── rules.engine.ts
│       │   │
│       │   ├── monitoring/
│       │   │
│       │   ├── stellar/
│       │   │   ├── stellar.service.ts
│       │   │   ├── soroban.service.ts
│       │   │   └── transaction.service.ts
│       │   │
│       │   ├── notifications/
│       │   │
│       │   ├── prisma/
│       │   │
│       │   └── main.ts
│       │
│       └── package.json
│
├── contracts/
│   │
│   └── treasury-vault/
│       ├── src/
│       │   ├── lib.rs
│       │   ├── contract.rs
│       │   ├── storage.rs
│       │   ├── errors.rs
│       │   └── types.rs
│       │
│       ├── tests/
│       │   └── treasury_test.rs
│       │
│       ├── Cargo.toml
│       └── README.md
│
├── packages/
│   ├── shared/
│   ├── types/
│   └── config/
│
├── scripts/
│   ├── deploy-contract.ts
│   └── initialize-treasury.ts
│
├── docs/
│   ├── architecture.md
│   ├── soroban-contract.md
│   ├── agent.md
│   └── security.md
│
├── .env.example
├── docker-compose.yml
├── package.json
└── README.md
🔄 Example Transaction Flow
1. User connects Stellar wallet
             ↓
2. User creates treasury
             ↓
3. User deposits USDC
             ↓
4. Soroban contract holds/manages treasury
             ↓
5. Backend monitors treasury
             ↓
6. AI analyzes activity
             ↓
7. AI identifies an opportunity
             ↓
8. AI creates recommendation
             ↓
9. User approves OR automation rule applies
             ↓
10. Soroban contract validates request
             ↓
11. Stellar executes transaction
             ↓
12. Transaction is recorded
             ↓
13. AI updates treasury analysis
🧪 Example AI Interaction
User

How is my treasury doing?

AI

Your treasury currently holds approximately 17,000 USDC. Your recent spending is within normal levels, but your reserve balance is below the target you configured.

User

Show me unusual transactions.

AI

I found one transaction that requires attention. A 5,000 USDC outgoing transaction is significantly larger than your recent average of 350 USDC.

User

What should I do?

AI

I recommend reviewing the transaction before allowing additional automated payments.

User

Move 200 USDC to my reserve wallet.

AI

The transaction is within your configured 500 USDC limit and the destination is an approved Stellar address.

Approve Transaction

📊 Treasury Health Score

An optional feature is an AI-generated treasury health score.

Example:

TREASURY HEALTH

        87 / 100

✓ Healthy liquidity
✓ Normal spending
✓ Good reserve level
⚠ High asset concentration

The AI explains the score:

Your treasury is healthy overall. However, 72% of your treasury is concentrated in one asset. Consider maintaining a more diversified reserve.

The score is intended as an informational tool, not financial advice.

🌍 Why Stellar?

Stellar is particularly suitable for treasury and payment applications because the network is designed around efficient digital-asset transfers and payments.

For this project, Stellar provides:

Fast settlement
Low-cost transactions
Stablecoin payments
Native asset infrastructure
Soroban smart contracts
Programmable on-chain treasury controls

The combination allows us to build a treasury system where AI can operate financial workflows while Soroban enforces the rules.

🎯 What Makes This Different?

A normal AI financial assistant looks like:

User
 ↓
AI
 ↓
Answer

A normal crypto wallet looks like:

User
 ↓
Wallet
 ↓
Transaction

AI Treasury Agent combines both:

User
 ↓
AI Treasury Agent
 ↓
Analyze
 ↓
Recommend / Automate
 ↓
Soroban Smart Contract
 ↓
Validate Permissions
 ↓
Stellar
 ↓
Execute

The AI is therefore connected to real programmable financial infrastructure.
