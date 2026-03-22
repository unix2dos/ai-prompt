# AGENTS.md

## Cursor Cloud specific instructions

This is a **documentation-only repository** (AI Prompt knowledge base) with no application services, no build system, and no package dependencies.

### Repository structure

- `1_学习知识/`, `2_解决方案/`, `3_技术相关/`, `4_有意思存档/` — Markdown content organized by category.
- `Alfred_Code.md`, `Alfred_Study.md`, `Alfred_Tool.md` — Auto-generated from Alfred snippets; do not edit manually.
- `sync_alfred_prompts.py` — Python 3.10+ script (stdlib only) that syncs Alfred snippets to Markdown. Requires macOS Alfred snippet directory at `~/workspace/vault/alfred/Alfred.alfredpreferences/snippets`; runs gracefully when that path is absent.

### Development

- **No dependencies to install.** No `package.json`, `requirements.txt`, or similar.
- **No services to start.** No dev server, database, or build step.
- **Lint/test:** There are no linters or test suites configured. You can validate the Python script with `python3 -m py_compile sync_alfred_prompts.py`.
- **Running the script:** `python3 sync_alfred_prompts.py` (will report missing folders on non-macOS environments — this is expected).
