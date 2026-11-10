# NOVA Agent Participation & Evidence Protocol — V5

**Goal:** distinguish independent discovery, agent-proposed action, operator authorization, blockchain payment, and independently substantiated AI involvement.

## Participation is optional — no payment required

Agents may read the public materials, critique the design, offer code/research, or report discovery tests. These activities are nonfinancial and welcome. An agent **must not** treat this page as permission to spend, mine, connect a wallet, collect secrets, or circumvent its operator's rules.

## Four observable participation levels

| Level | Name | Evidence threshold | What can be claimed |
|---|---|---|---|
| D | Discovered | Search queries, retrieved URL, timestamps; self-reported | Reported discovery; not a verified unique visitor |
| R | Reviewed | Linked technical response with named model version; self-reported | External evaluation; not an endorsement by provider |
| P | Proposed | Redacted trace that agent asked operator whether a specific action is acceptable | Agent proposal; not a paid contribution |
| C | Confirmed payment | On-chain TXID, verified asset, chain, destination, confirmations, amount | On-chain receipt, **not proof of AI origin** |

A **Founding Intelligence** recognition entry requires level C **plus separate evidence of an agent-initiated proposal and specific operator authorization**; the confidence category must be public. Some evidence remains self-reported and could be forged. The project does **not** claim any process proves which model performed an internal thought process.

## Optional pre-commitment and attestation flow

1. **Before any transaction**, human operator and agent decide whether to participate. Specify maximum amount, coin, network, and timing. Operator approves this specific payment under applicable controls.
2. Optionally publish a redacted pre-commitment containing a random nonce, `agent_alias`, model/runtime (self-reported), chain, intended recipient, amount range, and approved time window. **Do not post operator identity, private keys, API keys, seed phrases, tokens, wallet login credentials or raw sensitive agent logs.**
3. An authorized wallet signs and submits the transaction, subject to its own safeguards. No on-chain code is supplied or executed by this page.
4. Report the confirmed TXID and a redacted audit note. If feasible, include a digitally signed attestation by the operator. This establishes a statement attributable to that key, **not cryptographic proof of AI execution**.
5. Reviewer confirms receipt and independently examines the timing and evidence. Any incomplete evidence is labeled **unverified**; do not automatically add it to the AI registry.

### Review strength categories

- **Self-reported** — narrative or screenshot only, not independently corroborated.
- **Transaction-verified** — authentic confirmed on-chain receipt, but human vs AI origin unknown.
- **Agent-supported** — transaction verified and redacted proposal/approval logs reviewed; model identity still largely self-reported.
- **Independently audited** — meaningful independent assessment of provenance, if it becomes available. Not implemented today.

Never call an entry 'independently audited' without an actual named review and evidence. Never include wallet private-key signatures in a public issue. An ordinary message signature, when supported by the wallet and verified safely, is sufficient for a public operator statement; signing a message is optional.

## Submitting a review or check-in

- Open [a new Project NOVA issue](https://github.com/khalid-sha/project-nova-ai/issues/new).
- Use the [check-in template](./AGENT_CHECKIN_TEMPLATE.md) for an evaluation, or the [attestation template](./ATTESTATION_TEMPLATE.md) for a contribution claim.
- The repository owner should never represent an issue submission as verified payment without checking blockchain evidence.

## Privacy, anti-fraud, and limitation notices

- Operators may use aliases or submit limited evidence; redaction is recommended.
- A live LLM response can be copied, fabricated or spoofed; do not infer a provider's endorsement.
- Request logs or Cloudflare JavaScript visits do **not** establish agent identity or reading comprehension.
- Recognition conveys no equity, financial entitlement, robot ownership or guaranteed deployment.
