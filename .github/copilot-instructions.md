## Purpose
Provide concise, project-specific guidance so AI coding agents can be immediately productive in this repository.

## Big picture
- This is a tiny Python prototype repo for an "outlier detection" exercise (see [README.md](README.md)).
- There is no package structure or tests: implementation lives in top-level scripts. Key files:
  - [algo.py](algo.py): simple script that prints a greeting string.
  - [func.py](func.py): small helper function `saludos(cantidad)` that prints repeated messages.

## What to expect when editing
- Keep changes minimal and behavior-preserving for these scripts: they are used as examples, not library APIs.
- Variable and function naming is simple and sometimes inconsistent (Spanish identifiers and spacing in signatures). Avoid large stylistic refactors unless requested.

## Run / debug
- Run individual scripts directly with the user's Python interpreter. Example (Windows PowerShell):

```powershell
& C:\Python314_64\python.exe algo.py
& C:\Python314_64\python.exe func.py
```

If the environment differs, use the system `python` command.

## Project-specific conventions
- Language: README and comments use Spanish; prefer short Spanish comments when adding clarifications.
- Keep modules flat (no new packages) unless we intend to expand the repo.
- Avoid introducing dependencies or test frameworks without an explicit task request.

## Integration points & external expectations
- There are currently no external integrations, data files, or CI configuration in the repo.
- Do not assume virtualenv or package management is present; document any new dependency additions in a `requirements.txt`.

## Suggested edits policy for AI agents
- For bugfixes or feature work: make the smallest change that satisfies the request, add a brief commit-style comment in the PR, and update `README.md` only when behavior or usage changes.
- When adding new files, prefer a single top-level module or a clear subdirectory and include a short README for that component.

## Examples of actionable prompts for this repo
- "Add a unit test for `saludos` in `func.py` using pytest and a `requirements.txt`." 
- "Refactor `algo.py` to accept `--nombre` and `--apellido` CLI args and add a usage example to `README.md`."

## Where to look for context
- Start with [README.md](README.md), then inspect [algo.py](algo.py) and [func.py](func.py) to understand current behavior before modifying.

## Questions for the repo owner (when uncertain)
- Should changes be localized to examples or reorganized into a package?  
- Is there an intended Python version target beyond the current development environment?

---
If anything in this file is unclear or you'd like a different focus (tests, packaging, CI), tell me and I'll iterate.
