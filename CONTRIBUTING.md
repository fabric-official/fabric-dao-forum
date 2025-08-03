Contributing to Fabric DAO Forum

Thank you for contributing to Fabric DAO Governance.
This document explains how to create proposals, discuss governance changes, and participate in voting to help shape the future of the Fabric 1.0 ecosystem.

📝 Submitting a Proposal

Fork this repository or create a new branch.
Create a new YAML file in the proposals/ folder:
id: DAO-XXX
title: "Proposal Title"
summary: "One-sentence summary of the proposal."
details: |
  Full explanation of the problem, proposed solution, and impact.
impact:
  - Key impact 1
  - Key impact 2
Commit and push the new proposal:
git add proposals/DAO-XXX.yaml
git commit -m "Add DAO-XXX proposal"
git push origin main
Once merged, a GitHub Action automatically creates a DAO Forum Discussion.

💬 Participating in Discussions

Navigate to Discussions → Governance Proposals
Read active proposals and their details
Provide constructive feedback and suggestions
Collaborate with authors to refine proposals before voting

🗳️ Voting on Proposals

All voting happens on-chain to ensure cryptographic transparency.
Vote via CLI
fab dao vote --proposal DAO-XXX --choice yes
or:
fab dao vote --proposal DAO-XXX --choice no
Check Voting Status
fab dao vote status --proposal DAO-XXX

🔑 Proposal Lifecycle

Draft Stage: Proposal created in /proposals/
Discussion Stage: Automated GitHub Discussion thread
Voting Stage: Members cast votes on-chain
Execution Stage: Approved proposals automatically update:
Royalty policies
DAO treasury allocation
XP multipliers
Governance rules

✅ Best Practices

Keep proposals clear and concise
Include specific changes and measurable outcomes
Tag proposals with appropriate labels for categorization
Avoid duplicates—search existing proposals first
Respect DAO governance principles: transparency, fairness, decentralization

🤝 Code of Conduct

We maintain a professional, inclusive environment.
By participating, you agree to:
Communicate respectfully
Focus on constructive collaboration
Avoid spam or malicious proposals

🔐 Security Disclosures

If you discover a security vulnerability, do not post it publicly.
Report privately to the Fabric DAO Security Working Group.

📜 License

Contributions are governed by the Fabric DAO open governance license.
By submitting proposals, you agree to their public, immutable storage and execution.
© 2025 Atomic Limited – Fabric DAO Governance
