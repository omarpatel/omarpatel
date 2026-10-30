# Omar Patel

High school student in Waterloo, Ontario. I write Solana programs in Rust, contracts in Solidity, trading systems in Python, and the TypeScript apps around them.

[LinkedIn](https://www.linkedin.com/in/omarpateldev/) / [omarpatel.github.io](https://omarpatel.github.io)

### Founded

In 2026 I founded and launched 8 on-chain products on Solana and Robinhood Chain. Most are offline now; the code for several is public below.

- [Imagine](https://imagine.fun): lock-to-earn vaults for Raydium LaunchLab coins. 15 coins, $6.6k paid out to 37 wallets in 423 on-chain payouts.
- Pyre: AI app builder where each app is funded by its own coin. $800k+ on-chain volume, 700+ holders. Code: [prompt-to-app-platform](https://github.com/omarpatel/prompt-to-app-platform).
- Clasp: lock-to-earn launchpad on Robinhood Chain. 6 coins, 2.4+ ETH claimed by lockers.
- Coffer: non-custodial trader vaults on Solana. $380k+ token volume; the vaults never took outside deposits. Code: [trader-vaults](https://github.com/omarpatel/trader-vaults).
- Backstock: backer-funded launches on Raydium LaunchLab. 9 launches, $300k+ token volume.
- [KOL Brain](https://kolbrain.fun): AI profiles of Solana wallets' trading styles. $200k+ token volume. Code: [wallet-behavior-graph](https://github.com/omarpatel/wallet-behavior-graph).
- PaperApe: paper trading for Solana memecoins. Code: [paper-trading-platform](https://github.com/omarpatel/paper-trading-platform).
- Bellwether: fee-to-buyback engine, run as a paper-mode beta. Code: [fee-treasury-perps-engine](https://github.com/omarpatel/fee-treasury-perps-engine).

### Solana programs

- [trader-vaults](https://github.com/omarpatel/trader-vaults): investors pool SOL, a trader trades it, and the Anchor program gives the trader no way to withdraw it.
- [copy-trade-vault-program](https://github.com/omarpatel/copy-trade-vault-program): vaults that copy a public wallet's trades, but only after the program re-checks each signal on-chain.
- [onchain-economy-sim](https://github.com/omarpatel/onchain-economy-sim): multiplayer economy game on a deterministic tick server, settled through four Anchor programs.
- [solana-name-registry](https://github.com/omarpatel/solana-name-registry): @handles that resolve to Solana wallets. Anchor program, API and web app.

### Solidity

- [leveraged-treasury-engine](https://github.com/omarpatel/leveraged-treasury-engine): a token's fees go into a leveraged treasury on Uniswap v4, and only realized gains fund buybacks. 96 Foundry tests including invariants.
- [twab-stock-dividend-distributor](https://github.com/omarpatel/twab-stock-dividend-distributor): pays holders in tokenized stocks by time-weighted balance, through Merkle rounds. 57 Foundry tests.
- [fee-split-vaults-postmortem](https://github.com/omarpatel/fee-split-vaults-postmortem): creator-fee split vaults, plus the on-chain market study that made me shelve the launch.

### Trading and AI agents

- [llm-trading-arena](https://github.com/omarpatel/llm-trading-arena): seven LLMs and three code baselines each trade their own Solana wallet. A `/proof` page reconciles the ledger against on-chain balances.
- [agent-treasury](https://github.com/omarpatel/agent-treasury): AI agents that pay for their own LLM calls out of a Solana treasury and die when it runs out.
- [prompt-to-app-platform](https://github.com/omarpatel/prompt-to-app-platform): turns a one-sentence prompt into a hosted web app, built by the Claude Agent SDK in E2B sandboxes. 529 tests.
- [fee-treasury-perps-engine](https://github.com/omarpatel/fee-treasury-perps-engine): turns fee income into US-equity perp trades and buybacks, with a double-entry ledger. Paper mode by default.
- [wallet-behavior-graph](https://github.com/omarpatel/wallet-behavior-graph): profiles Solana wallets into trading styles and maps which wallets lead and which follow.
- [ibkr-algo-trader](https://github.com/omarpatel/ibkr-algo-trader): Interactive Brokers paper trading with walk-forward backtests, an XGBoost trade filter and a kill switch.
- [ibkr-live-dashboard](https://github.com/omarpatel/ibkr-live-dashboard): read-only IBKR P&L and positions, streamed to the browser over WebSocket.

### Payments and apps

- [fee-routed-fundraising](https://github.com/omarpatel/fee-routed-fundraising): creator fees swapped to USDC and paid to a fundraiser, with a SHA-256 receipt anchored on Solana for every delivery.
- [solana-invoicing](https://github.com/omarpatel/solana-invoicing): payment links, milestone escrow, swaps, multisig and split payments on Solana.
- [crypto-checkout-extension](https://github.com/omarpatel/crypto-checkout-extension): a Chrome extension that pays card checkouts from a USDC or SOL balance.
- [paper-trading-platform](https://github.com/omarpatel/paper-trading-platform): one Express/WebSocket API behind a Next.js app, an Expo app and a Chrome extension.
- [dlmm-liquidity-explorer](https://github.com/omarpatel/dlmm-liquidity-explorer): concentrated-liquidity pools ranked by fee yield on a three.js map.
- [multiplayer-snake-arena](https://github.com/omarpatel/multiplayer-snake-arena): real-time multiplayer snake on an authoritative Socket.IO server, with bots.

### Tools

- [live-call-subtitles](https://github.com/omarpatel/live-call-subtitles): offline English subtitles for any Windows voice call, using Whisper on the GPU.
- [deployer-forensics](https://github.com/omarpatel/deployer-forensics): zero-dependency CLI that scores a pump.fun creator wallet for automated extraction patterns.
- [hd-wallet-sweeper](https://github.com/omarpatel/hd-wallet-sweeper): dry-run-first recovery of funds from BIP32/BIP39-derived EVM and Solana addresses.
- [vanity-address-grinder](https://github.com/omarpatel/vanity-address-grinder): multi-core vanity address grinder for Solana and Ethereum.

Every repo has a demo mode or local setup and CI that runs its own tests.
