# AGENTS.md

## Project role
This repository is a small archival utility for preserving public Perth Priority Removals website pages in the Internet Archive. Keep it simple, low-maintenance, and narrowly scoped to archiving.

## Default work style
- Make minimal targeted changes.
- Preserve the existing archival purpose and workflow.
- Do not add unrelated crawling, scraping, analytics, SEO, or content-modification features unless explicitly requested.
- Avoid unnecessary dependencies and complexity.
- Prefer reversible changes and small diffs.

## Implementation rules
- Respect archive.org rate limits and existing crawl-delay protections.
- Do not expand crawl scope beyond intended public PPR pages without explicit approval.
- Do not submit private, authenticated, staging, admin, or sensitive URLs to third-party archives.
- Preserve manual and scheduled workflow behaviour unless the ticket specifically changes it.
- Keep configuration explicit and reviewable.

## Testing and verification
- Run the most relevant available checks before completion.
- If live archive submission is not appropriate for a test, use safe/dry verification and say so.
- Do not claim a Wayback snapshot succeeded unless verified.
- Report changed files, tests run, risks/assumptions, and anything not completed.

## Markdown and durable context
- Proactively recommend creating or updating the appropriate `.md` file when work produces durable project context, workflow rules, decisions, constraints, architecture knowledge, or reusable instructions.
- Name the specific file that should change and state what should be added, changed, or removed.
- Prefer updating an existing authoritative file over creating a duplicate or competing source of truth.
- Keep repository-specific implementation rules in `AGENTS.md` or the appropriate project `.md` file.
- Update relevant context documentation when an implementation materially changes a durable assumption or operating rule.
- Do not place private health, family, faith, client-identifying, or unrelated personal information into repository documentation.

## Security and privacy
- Never print or commit secrets, tokens, API keys, private client details, or `.env` contents.
- Treat logs and archived URLs as potentially sensitive until confirmed public.
