Fabric DAO Forum
Welcome to the Fabric DAO Forum – the decentralized governance hub of the Fabric 1.0 ecosystem.
This repository powers on-chain proposals, automated Discussions, and DAO-driven decision-making for Fabric’s future.
🌐 Overview
DAO Governance: Fully decentralized proposal and voting system
Automated Discussions: Every proposal creates a public discussion thread
On-Chain Execution: Approved proposals update policies, royalties, and treasury flows
Transparency: Immutable history of every governance decision
📂 Repository Structure
fabric-dao-forum/
│
├── proposals/                   # Governance proposals in YAML format
│   ├── DAO-001.yaml              # Genesis Royalty Distribution
│   ├── DAO-002.yaml              # XP Multiplier for Early Developers
│   └── DAO-003.yaml              # Treasury Allocation for Bounty Program
│
├── .github/
│   └── workflows/
│       └── dao-proposal.yml      # GitHub Action → auto-create Discussions
│
└── README.md                     # This file
🗳️ Submitting a Proposal
To submit a proposal:
Create a new .yaml file in the proposals/ folder
Use the following structure:
id: DAO-XXX
title: "Proposal Title"
summary: "Short summary of proposal."
details: |
  Full description of what the proposal aims to achieve.
impact:
  - Key impact 1
  - Key impact 2
Commit and push to the repository:
git add proposals/DAO-XXX.yaml
git commit -m "Add DAO-XXX proposal"
git push origin main
🤖 Automated Discussions
Each new proposal triggers the DAO Proposal GitHub Action
This creates a public Discussion thread in the DAO Forum
Members can debate and refine proposals before voting on-chain
🗳️ Voting
Voting happens on-chain via the Fabric CLI:
fab dao vote --proposal DAO-001 --choice yes
Check results:
fab dao vote status --proposal DAO-001
💰 Treasury and Rewards
Approved proposals can allocate DAO treasury funds
Rewards are claimed via:
fab claim
📜 Current Proposals
ID	Title	Status
DAO-001	Genesis Royalty Distribution Framework	🟢 Active
DAO-002	XP Multiplier for Early Developers	🟢 Active
DAO-003	Treasury Allocation for Bounty Fund	🟢 Active
✅ Contribution
Fork this repo
Add your proposal or improvements
Open a pull request
Engage in Discussions
🔐 Governance Principles
Transparency: All decisions are public and immutable
Fairness: Every DAO member has equal rights to propose and vote
Decentralization: No central authority can override DAO votes
© 2025 Atomic Limited – Powered by Fabric DAO Governance
