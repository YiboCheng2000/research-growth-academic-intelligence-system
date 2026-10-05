# GitHub publishing checklist

This file is for the maintainer preparing the first public repository.

## Recommended repository metadata

**Repository name**

`research-growth-academic-intelligence-system`

**Description**

> Evidence-grounded research growth and academic-intelligence workflow with source verification, contradiction search, deduplication, contribution mapping, and cross-platform AI adaptation.

**Suggested topics**

`academic-research` `literature-review` `research-workflow` `research-assistant` `prompt-engineering` `chatgpt` `agent-skills` `academic-writing` `evidence-grounding` `scholarly-communication`

## Clean-history publication path

Use a **new** Git repository for the sanitized public release if any predecessor contained private information.

Example:

```bash
cd Research_Growth_Academic_Intelligence_System_v1.0.0
rm -rf .git
git init
git branch -M main
git add .
git status
git diff --cached --stat
git commit -m "release: v1.0.0 public launch"
git tag -a v1.0.0 -m "v1.0.0 first public release"
```

Then create the GitHub repository and add its remote using the URL GitHub gives you.

Before pushing:

1. Run a final secret scan on the exact staged tree.
2. Read `git diff --cached` for accidental private data.
3. Confirm no `.env`, private profile, exported email, task ID, participant data, or unpublished private file is staged.
4. Confirm `LICENSE`, `ATTRIBUTION.md`, `THIRD_PARTY_NOTICES.md`, and `DISCLAIMER.md` are included.

## GitHub Release

Create a release from tag `v1.0.0` and use `RELEASE_NOTES_v1.0.0.md` as the starting body.

## Post-push verification

Open the repository in an incognito/logged-out browser and inspect:

- README rendering;
- repository description and topics;
- license visibility;
- release tag;
- issue templates;
- raw prompt files;
- Git history;
- any unexpectedly indexed personal information.

If sensitive information is discovered after publication, treat credentials as compromised where applicable and remove the sensitive value from Git history rather than only deleting it from the latest commit.
