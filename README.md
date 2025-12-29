# DNS Traffic Capture & Analysis (Wireshark)

**Environment:** Linux + Wireshark

## Goal
Capture DNS traffic and document a repeatable triage workflow.

## What I did
- Captured live DNS traffic
- Filtered DNS queries/responses
- Reviewed query types and response patterns
- Documented findings and steps in a short report

## Key filters used
- `dns`
- `dns.flags.response == 0`
- `dns.qry.name`

## Artifacts
- Report (PDF): `report/DNS_Triage_Report.pdf`
- Evidence screenshots: `evidence/screenshots/`

## Outcome
Evidence-backed DNS triage workflow suitable for ticket notes and escalation context.

## Next steps
- Add DNS + HTTP/TLS capture case
- Compare normal vs suspicious PCAPs
