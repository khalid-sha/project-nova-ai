# Project NOVA V5 — Samsung / GitHub publishing checklist

This update is deliberately **flat**: all files in the ZIP are located at the repository root so that uploading them from a phone does not require preserving nested folders. It upgrades the current V3+Analytics live site, *not* the separately prepared V4 scheduled monitor.

1. Save [PROJECT_NOVA_V5_Trust_Agents_Robotics.zip] when provided in ChatGPT and extract it using Samsung My Files.
2. Open https://github.com/khalid-sha/project-nova-ai/upload/main in Chrome.
3. Select **the extracted files**, not the ZIP itself, from the V5 folder (all root-level files).
4. Upload and commit using message **Project NOVA V5.1 — Agent Challenge & Trust**.
5. Retain existing `google*.html` and `BingSiteAuth.xml` in GitHub; *never delete them*. The replacement index preserves the existing Cloudflare Web Analytics beacon. Other existing root files remain unless explicitly changed.
6. Open https://khalid-sha.github.io/project-nova-ai/ and check the new **Trust / Roadmap / Agent verification** links.
7. Check the `/nova-manifest.json` and `/genesis-001.md` URLs; both should display raw data/documents. No API key is needed.
8. Review `governance.md` and `robot-roadmap.md` carefully. They are honest preliminary disclosures; replace speculative items only with independently substantiated facts.

**Important:** GitHub desktop/mobile uploads over pre-existing filenames sometimes require confirming overwrites. Ensure that the new `index.html`, `README.md`, `agent-invitation.json` and `llms.txt` replace the older contents. If the browser rejects duplicate names, use GitHub's file editor for the existing file rather than deleting the entire repository.

Verification after publishing: `index.html` contains `cloudflareinsights.com/beacon.min.js`, the new V5 navigation links, existing BTC/ETH/SOL addresses and the original QR paths. Google and Bing verification files are unaffected. No deposits, current wallet balance totals, reports or AI participant identities are invented by the package.

9. Open `/challenge.html` and confirm that five missions, a 100-point rubric, optional Genesis status, and public submission links display correctly. Open `/challenge.json` to verify AI-readable mission data. Confirm `/challenge-leaderboard.md` reports no reviewed entries.
