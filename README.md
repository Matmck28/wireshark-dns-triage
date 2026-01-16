# DNS Traffic Capture & Triage (Wireshark)

## Environment
- Linux
- Wireshark

## Objective
Capture DNS traffic and document a repeatable triage workflow (queries, responses, and NXDOMAIN cases).

## Repo structure
- `report/` — short write-up (PDF or markdown)
- `evidence/screenshots/` — sanitized screenshots used as proof of work

## Method
1. Start a capture on the active interface (e.g., `wlp2s0`)
2. Generate DNS activity (browse to a site + run a few test lookups)
3. Apply display filters to isolate DNS behavior
4. Identify query types (A/AAAA) and response outcomes (NOERROR vs NXDOMAIN)
5. Document observations as ticket-style notes

## Key Wireshark filters used
- `dns`
- `dns and udp.port ==

