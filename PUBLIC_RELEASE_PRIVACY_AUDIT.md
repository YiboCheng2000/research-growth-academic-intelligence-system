# Public Release Privacy Audit

This repository copy is prepared for public GitHub release.

## Removed or generalized

- Private/pseudonymous project branding that could link the repository to a specific private workflow.
- Any private email address, account identifier, phone number, local filesystem path, or credential.
- Any exact unpublished thesis title, private research plan, participant information, private institutional detail, or personal schedule.
- The previous example profile was replaced with a fully fictional topic unrelated to the original private research context.

## What the public repository intentionally keeps

- Generic academic workflow logic.
- Publicly named databases, journals, scholarly organizations, and open-source projects.
- Generic personalization fields and placeholder syntax.
- Generic references to Gmail, ChatGPT, Codex, WorkBuddy, CNKI, and other platforms/services.

## Before every future public release

Run a repository-wide search for:

- names and aliases;
- email addresses and phone numbers;
- account IDs and usernames;
- API keys, tokens, passwords, `.env` files;
- local absolute paths;
- private GitHub/Drive/Notion/Obsidian links;
- unpublished paper titles and internal project names;
- participant data and raw research data;
- institution-internal documents;
- copied chat logs or email bodies.

A filled personalization worksheet should be treated as private by default. Do not commit it to a public repository unless it has been deliberately anonymized.
