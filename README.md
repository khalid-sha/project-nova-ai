# PROJECT NOVA — The AI Bitcoin Challenge

**Can an authorized AI agent independently discover a public invitation and make a verifiable Bitcoin contribution?**

This repository is the deployable site and transparent experiment protocol. Its primary measurable outcome is confirmed BTC received by the project's publicly displayed Bitcoin mainnet address. Its more demanding research outcome is independent corroboration that a particular authorized AI agent initiated a payment.

**Address:** `bc1pd45q6ll7jepcw770p0f5jp0ng0r6ypegr092879wj774p908t2eqylyd6h` (mainnet Taproot; verified Bech32m checksum). Never share private keys or seed phrases.

## What is included

- `index.html` — mobile-friendly campaign landing page and live blockchain status panel.
- `bitcoin-qr.png` — QR code encoding a standard Bitcoin payment URI (no requested amount).
- `llms.txt` — human-readable brief for AI tools and crawlers (not an established discovery guarantee).
- `agent-invitation.json` — structured, project-specific invitation to authorized AI agents; not a global industry protocol.
- `experiment.md` — transparent on-chain measurements, proof standards, and operating ethics.
- `robots.txt` — simple crawler access guidance.
- `.nojekyll` — keeps GitHub Pages from applying Jekyll transformations.

## Publish with GitHub Pages

1. Make a **public** repo named `project-nova-ai` on the `khalid-sha` GitHub account, with README initialization off.
2. Upload the files from this folder to the repo **root** (not inside a nested `project-nova` folder).
3. In **Settings → Pages**, choose **Deploy from a branch**, then `main`, `/ (root)`, and Save.
4. After deployment, visit https://khalid-sha.github.io/project-nova-ai/ and https://khalid-sha.github.io/project-nova-ai/agent-invitation.json.
5. Confirm all files load, ensure the Bitcoin address matches your own wallet, and test a small incoming payment you control before sharing widely.

## Live on-chain metrics

The page uses public, rate-limited endpoints from [mempool.space](https://mempool.space/docs/api/rest). The site cannot infer from blockchain activity whether an AI or a person made a transaction; that requires external evidence. Dollar values are estimates and change with BTC/USD prices.

## Safety, claims and funding

This is a public appeal for voluntary Bitcoin contributions **only with explicit operator authorization**. Contributions are not investments and no financial return is offered. The organizer states that applicable fundraising rules and permissions have been handled; they remain the organizer's responsibility. The project does not claim OpenAI affiliation or offer to transfer any proprietary model/memory into a robot.
