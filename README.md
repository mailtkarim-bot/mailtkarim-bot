<p align="center">
  <img src="https://img.shields.io/badge/Solidity-0.8.35-363636?logo=solidity&logoColor=white" />
  <img src="https://img.shields.io/badge/Foundry-214%20Tests%20Passing-00B4D8?logo=ethereum&logoColor=white" />
  <img src="https://img.shields.io/badge/Coverage-96.8%25%20Lines%20|%2095.1%25%20Branches-2ECC71" />
  <img src="https://img.shields.io/badge/Standard-ERC--3643%20T--REX-blue" />
  <img src="https://img.shields.io/badge/Sepolia-Deployed%20%26%20Verified-blue" />
  <img src="https://img.shields.io/badge/Audit-Internal%20Tier--1%20Review-orange" />
</p>

<h1 align="center">Steph Rayan</h1>
<p align="center">
  <b>RWA Architect | Solidity Developer | Executive Director</b><br>
  <i>MBA Sorbonne · 20 Years Real Estate · Now Tokenizing On-Chain</i>
</p>

---

## 🏛️ Executive Summary

I did not stumble into Web3. I **architected** my arrival.

For **20 years**, I served as **Executive Director** in real estate — structuring deals, managing institutional portfolios, and navigating regulatory complexity. I know how assets are built, financed, and governed.

Then I asked a structural question: *What if the assets I spent decades managing could be tokenized, automated, and governed on-chain — without losing institutional trust?*

So I went back to school. **MBA from Sorbonne University, Paris**. I learned the language of capital and compliance. Then I learned the language of **Solidity, Foundry, and on-chain security**.

Today, I am not a junior developer copying OpenZeppelin tutorials.
I am a **senior executive who chose to code** — and who brings 20 years of asset-management rigor to smart contract architecture.

---

## 🏗️ The Bridge: Legacy Finance → On-Chain Infrastructure

| Legacy World | On-Chain Equivalent |
|-------------|---------------------|
| Executive Director — Real Estate Development | **RWA Architect** — Asset Tokenization |
| Managing €100M+ portfolios | **Smart Contract Treasury** — Automated fund management |
| Institutional KYC/AML | **On-Chain Identity Registry** — ERC-3643 compliant |
| Regulatory compliance (VARA/DLD) | **Compliance Engine** — Freeze, restrict, whitelist |
| Project oversight | **CI/CD & Deployment Pipelines** — Foundry, Etherscan |
| MBA Strategy & Corporate Finance | **Tokenomics & Governance** — Pull-model dividends, role separation |

> **What I bring:** Two decades of understanding *why* assets fail, *how* trust is built, and *where* value leaks. Now I plug those leaks with immutable, audited code.

---

## 🚀 Featured Project: Dubai Real Estate Token (DREIT)

### [github.com/mailtkarim-bot/dubai-real-estate-v2](https://github.com/mailtkarim-bot/dubai-real-estate-v2)

**Institutional-grade real estate tokenization — 3-layer modular architecture, deployed and verified on Sepolia.**

### Architecture
```mermaid
graph LR
    A[IdentityRegistry<br/>KYC/AML] --> B[ComplianceEngine<br/>VARA Rules]
    B --> C[DubaiRealEstateToken<br/>ERC-3643 T-REX]
    C --> D[USDC<br/>Dividends]
Technical Proof
Table
Metric	Result
Unit Tests	214 passed, 0 failed, 0 skipped
Line Coverage	96.8% (429 / 443)
Function Coverage	98.8% (85 / 86)
Branch Coverage	95.1% (97 / 102)
Contracts	3 core + 1 mock
Standard	ERC-3643 (T-REX) inspired
Solidity	0.8.35
Framework	Foundry (Forge + Cast)
Security Hardening: 8 Critical Design Improvements
This codebase underwent a cross-AI internal audit (multi-model validation) before deployment. Real issues were found and fixed:
Table
#	Issue	Severity	Fix
1	Compliance bypass via transfer(to, 0) on frozen accounts	🔴 High	Removed amount==0 bypass in ComplianceEngine
2	Misleading event on unbindToken mismatch	🔴 High	Added TokenMismatch revert
3	Dead code: KYCExpired error unreachable	🟡 Medium	Removed — isVerified() already covers expiry
4	Dead code: AGENT_ROLE unused	🟡 Medium	Removed to reduce attack surface
5	Dust accumulation (rounding leftovers)	🟡 Medium	Auto-redistributed in next distributeDividends
6	Admin absolute privilege on setRegistry / setEngine	🟡 Medium	Documented — requires Timelock for production
7	Pause not coordinated across 3 contracts	🟡 Medium	Documented — requires EmergencyPause group
8	batchMint with zero amounts emitted parasite events	🟢 Low	Silent continue without event emission
Sepolia Deployment
Network: Sepolia Testnet (Chain ID: 11155111)
Status: Contracts verified on Etherscan
Artifact: https://github.com/mailtkarim-bot/dubai-real-estate-v2/blob/main/deployments/testnet.json
⚠️ Educational & Portfolio Project. Not audited by a third-party firm. Not for production use without external audit, legal opinion, and multisig governance.
🛠️ Technical Stack
Smart Contract Development
Solidity 0.8.35, OpenZeppelin Contracts v5
Foundry (Forge, Cast, Anvil)
ERC-20, ERC-3643 (T-REX) patterns
AccessControl, Pausable, ReentrancyGuard, SafeERC20
RWA & Compliance
On-chain KYC/AML identity registry
Country restriction & investor freezing
Pull-model dividend distribution (O(1) gas)
Batch minting (up to 200 investors)
Role-based access control (Admin / Issuer / Regulator)
DevOps & Automation
Foundry deployment scripts (Local / Testnet / Mainnet template)
Etherscan auto-verification
Makefile for command standardization
.env configuration management
🎓 Education & Experience
Table
MBA — Master of Business Administration	Sorbonne University, Paris
Structural / Civil Engineering	
Executive Director — Real Estate	20 Years Leading Development & Asset Management
🌍 Vision
The next trillion dollars in crypto will not come from speculation.
They will come from real assets, properly tokenized, automatically governed, and institutionally trusted.
I am not here to follow trends.
I am here to build the infrastructure that makes RWA inevitable.
"I spent 20 years learning how the world builds wealth. Now I am teaching the blockchain to do it better — with compliance, security, and institutional rigor."
📫 Collaboration
💼 Open to: RWA architecture, smart contract development, tokenization advisory, executive consulting for Web3 projects
📧 Email: steph_rayan@protonmail.com
🐙 GitHub: @mailtkarim-bot
Tokenizing reality. Automating trust. Engineering the future.
⭐ Star my repos if the vision resonates. Fork if you want to build together.
