# CODEX_TICKET_TEMPLATE.md

Use this format before asking Codex to make code changes.

## Narrow implementation ticket

Repo:
MrSparkleWebsites/wayback-archiver

Objective
[One sentence. What must change?]

Context / evidence
- [Relevant decision, bug, screenshot, log, issue, or user report]

Allowed areas
- [Files/folders/components Codex may inspect/edit]

Non-goals
- Do not redesign.
- Do not change unrelated files.
- Do not change provider settings, secrets, hosting, scheduled jobs, or deployment configuration unless explicitly listed.

Guardrails
- Make minimal targeted changes.
- Preserve current archiving behaviour unless the task specifically changes it.
- Avoid heavy dependencies.
- Watch for rate limits and external request volume.
- If the task appears broader than described, stop and ask.

Acceptance criteria
- [Measurable outcome 1]
- [Measurable outcome 2]
- [Measurable outcome 3]

Verification
- Run relevant tests/build/lint.
- Report command output summary.
- If unable to test, explain why.

Report format
- Summary:
- Files changed:
- Tests run:
- Risks:
- Follow-up:

Last updated: 2026-09-29
