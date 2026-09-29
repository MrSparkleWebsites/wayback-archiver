# AGENTS.md

This repository uses ChatGPT for planning and Codex for implementation. Work should be narrow, practical, low-maintenance, and easy to review.

## Project
Wayback archiver utility.

## Default work style
- Make minimal targeted changes.
- Preserve current behaviour unless the task explicitly changes it.
- Do not redesign or refactor broadly without approval.
- Do not introduce new frameworks, services, databases, or providers without explicit approval.
- Do not expose secrets, tokens, API keys, private URLs, or `.env` values.
- Do not change provider, hosting, or deployment settings unless explicitly requested.

## Before editing
- Restate the objective.
- Identify likely files/areas.
- Identify non-goals.
- Stop if the task is ambiguous or broader than the ticket.

## Implementation rules
- Prefer small diffs.
- Preserve tests/build process.
- Add tests when changing logic.
- Avoid heavy dependencies unless clearly justified.
- Keep scripts simple and maintainable.

## Testing
- Run the most relevant tests/lint/build commands available.
- If tests cannot be run, explain why.
- Do not claim production or scheduled-job verification unless it was actually performed.

## Report format
After work, report:
- Summary
- Files changed
- Tests run
- Risks / assumptions
- Anything not completed
- Suggested next step, if any

## Stop conditions
Stop and ask before continuing if:
- A secret, API key, provider setting, or dashboard action is required.
- The task could trigger external requests, bulk operations, or rate-limit risk beyond what was requested.
- Production deployment or scheduled execution is required but not explicitly authorised.

## Supporting references
- `docs/CODEX_TICKET_TEMPLATE.md`
