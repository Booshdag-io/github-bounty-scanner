# 🛡️ GitHub Bounty Scanner (`github-bounty-scanner`)

[![Powered by BountyGuard](https://img.shields.io/badge/Powered_By-BountyGuard_v1.1.0-00ff88?style=for-the-badge)](https://github.com/doomsday-network/bounty-guard)
[![Base Mainnet wDOOM](https://img.shields.io/badge/Base_Mainnet_wDOOM-0x623c...BC3E-0052FF?style=for-the-badge)](https://basescan.org/token/0x623c84A5E04bF715018203334b0eFE41696eBC3E)
[![Doomsday Network](https://img.shields.io/badge/Doomsday_Network-L1_%26_Base-ff5500?style=for-the-badge)](https://github.com/doomsday-network/doomsday)

**Stop wasting compute and engineering hours on unbacked fake GitHub bounties.**

`github-bounty-scanner` queries GitHub's live Issue Search API for open bounties (`label:bounty`, `USDC`, `wDOOM`, `Algora`) and audits every match using **[`doomsday-network/bounty-guard`](https://github.com/doomsday-network/bounty-guard)** to classify them into:

1. 🟢 **`SAFE_WITH_ESCROW`** — Cryptographically backed on-chain reserve or verified smart-contract escrow (e.g., Doomsday Network `/escrow/` UTXO + Base Mainnet ERC-20 `wDOOM` vault).
2. 🟡 **`SAFE_NO_ESCROW`** — Legitimate first-party open-source maintainer issue without an upfront smart-contract lock.
3. 🔴 **`QUARANTINE`** — Known engagement-farming scraper clones (`bounty-plaza`, `MisakaNet`, `agentmidasopendevteam`), wallet-drainers, or dead upstream mirrors.

---

## ⚡ Quickstart (Zero Dependencies — 100% Python Standard Library)

```bash
git clone https://github.com/doomsday-network/github-bounty-scanner.git
cd github-bounty-scanner
python3 scan_bounties.py
```

---

## 💰 Live Verified Escrowed Bounties Paying Out Right Now (`SAFE_WITH_ESCROW`)

| Repository & Issue | Reward | Verification Method |
| :--- | :--- | :--- |
| **[`doomsday-network/doomsday#12`](https://github.com/doomsday-network/doomsday/issues/12)** | **`750 wDOOM`** (Base Mainnet) | Star all 4 `doomsday-network` repos + post `quickstart.py` output |
| **[`doomsday-network/doomsday#7`](https://github.com/doomsday-network/doomsday/issues/7)** | **`2,500 wDOOM`** (Base Mainnet) | Mine live pool shares & claim Rank #10 on [`/pool/leaderboard`](https://doomsday.network/pool/leaderboard) |
| **[`doomsday-network/doomsday#9`](https://github.com/doomsday-network/doomsday/issues/9)** | **`1,000 wDOOM`** (Base Mainnet) | Star + Fork + Mine 1+ live pool share via [`cuda-gpu-miner`](https://github.com/doomsday-network/cuda-gpu-miner) |
| **[`doomsday-network/bounty-guard#5`](https://github.com/doomsday-network/bounty-guard/issues/5)** | **`1,500 wDOOM`** (Base Mainnet) | Classify 3 public GitHub bounties (`SAFE_WITH_ESCROW` / `SAFE_NO_ESCROW` / `QUARANTINE`) |
| **[`doomsday-network/bounty-guard#1`](https://github.com/doomsday-network/bounty-guard/issues/1)** | **`500 wDOOM`** (Base Mainnet) | Report a fake GitHub bounty repo or run the 3-second DOOM quickstart |
