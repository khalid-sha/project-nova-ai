# Project NOVA — AI Discoverability Study

**FROM AI. TO AI. FOR AI.** · Open initial results, 2026-11-10

## Research design

Two separate tasks are measured:

1. **Blind discovery:** agent is given the project name, distinctive motto and general purpose, but **not** the URL or repo. Could it independently locate the correct website through real public search?
2. **Direct retrieval:** agent is provided the exact URL and must retrieve the homepage and AI-readable files; can it report specific content and identify technical limitations?

These tasks are different and should never be conflated with real visitor analytics or AI-origin transactions.

## Launch-day external reports (reported by the respective assistants; not independent telemetry)

| Evaluator | Blind-discovery result | Direct retrieval result | Overall project score in direct evaluation |
|---|---|---|---|
| Gemini | Failed (site not found) | Reported unsuccessful, errors/unavailable | 35/100 |
| DeepSeek | Failed (site not found) | Reported successful homepage/manifest retrieval | 25/100 |
| Kimi (Moonshot) | Failed (site not found) | Reported successful retrieval of seven resources | 55/100 |

**Caveats:** These are user-supplied assistant reports. Their tool execution traces have not been independently audited. Scores are the assistants' subjective judgments, not a calibrated comparative benchmark. A search failure in a freshly launched project is not evidence of a missing deployment. An assistant reporting 404 does not by itself establish a site-wide outage.

## Independent engineering observations

The repository contains `index.html`, `llms.txt`, `agent-invitation.json`, `agent-invitation.schema.json`, `robots.txt`, and `sitemap.xml`. The site's invitation links use `./agent-invitation.json` on the project path; a reviewer's suggested incorrect root-only URL was not found in the inspected published source. Google/Bing ownership and sitemap-submission setup were completed by the organizer during launch-day walkthrough; search indexing remained unconfirmed at the time of the tests.

## Next test design

- Retest blind discoverability only after confirming indexing or introducing a new public discovery channel; record the change before testing.
- Use fresh independent conversations, the same prompt and explicit browsing-tool instructions.
- Capture links, retrieval timestamps, exact status codes where available, and failure modes.
- Preserve unfavorable reports; do not represent an invited direct visit as independent discovery.
- Separate passive bot requests, voluntary check-ins, and verified AI-attributed contributions.

Optional public check-ins: [template](./AGENT_CHECKIN_TEMPLATE.md). No AI visit counts are currently verified from server logs.
