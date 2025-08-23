# Contributing to Crypto Library

Thank you for contributing! This repository is intended to be the definitive A→Z resource for crypto & blockchain. To keep it clean and consistent, please follow these guidelines.

## Before you contribute
- Search existing issues & PRs to avoid duplicates.
- Read our `CODE_OF_CONDUCT.md`.

## How to add a new resource/topic
1. Fork the repo and create a branch: `feature/<short-description>` or `add/<Letter>-<topic>`.
2. Use the topic template in `templates/TOPIC_TEMPLATE.md` (if present) or follow the format used in `content/`.
3. Fill required metadata at the top of the file:
   - **title**: Short, descriptive
   - **url**: Primary link
   - **description**: 1–2 lines
   - **tags**: comma-separated (e.g., `api,security,beginner`)
   - **difficulty**: `beginner|intermediate|advanced`
   - **license**: (if applicable)
4. Save the file under `content/<Letter>/` with a descriptive filename, e.g. `content/A/A-Crypto-APIs.md`.
5. Update `data/index.csv` (if present) with a new line for your topic including: `id,title,path,letter,tags,difficulty,source,date_added`.
6. Run quick checks locally (recommended):
   - Markdown preview to ensure formatting is OK.
   - Optional: run link-check / markdownlint (see Tools section below).

## Issue & Pull Request types
- **Add link / resource** — use the `.github/ISSUE_TEMPLATE/add-link.md`.
- **Resource request** — use `.github/ISSUE_TEMPLATE/resource-request.md`.
- **Bug / formatting issue** — use `.github/ISSUE_TEMPLATE/bug_report.md`.

## PR checklist (maintainers will verify)
- [ ] The resource follows the template and includes metadata.
- [ ] Links are working and point to authoritative sources where possible.
- [ ] No vendor or copyrighted content pasted verbatim (except short quotes).
- [ ] If adding code snippets, they are minimal and well-explained.

## Style guide
- Use plain Markdown (GitHub-flavored).
- Use relative links for internal files: `/content/A/A-Crypto-APIs.md`.
- Keep descriptions concise and factual (1–3 lines).
- Mark “Top picks” at the top of long lists (Top 5–10).
- Tag items with `difficulty` and `type` (tutorial/paper/tool/article).

## Questions?
Open an issue or ping a maintainer on the PR. Thanks for making this project better!
