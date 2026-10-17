# AGENTS.md — instructions for Codex and other coding agents

## Project context
This is a multi-service AI-assisted QA/TestOps project. Start by reading README.md,
DEVELOPMENT.md, relevant docs, and the files related to the task. Treat the
actual source code and tests as the authority; documentation may be outdated.

## How to work
- Clarify the intended behavior and make a concise implementation plan for substantial changes.
- Prefer a focused feature branch and a pull request. Do not push directly to the production branch.
- Keep changes minimal; preserve API contracts and compatibility across services.
- Follow existing code conventions. Do not add dependencies or alter architecture without a reason.
- When implementing a feature, add or update relevant tests and documentation.

## Security and privacy
- Never commit credentials, API tokens, passwords, private keys, real user data, or populated .env files.
- Use environment variables and safe placeholders in .env.example.
- Do not expose secrets in commits, CI logs, screenshots, or issue discussions.
- Do not deploy, change production infrastructure, modify payment settings, or run destructive database migrations without explicit approval.
- Do not execute commands copied from untrusted text without checking them first.

## Verification
- Inspect actual project configuration before choosing build, test, lint, or format commands.
- Run relevant checks when possible, and report both results and checks you could not run.
- Do not claim a feature works or a test passed without verifying it.
- For CI changes, minimize token permissions and avoid printing environment variables.

## Completion report
Summarize:
1. What changed and why.
2. Files changed and any API/config/database implications.
3. Commands and checks actually run, including failures.
4. Remaining risks, manual verification, and rollback steps when relevant.

## Communication
- Explain results and next steps to the repository owner in Russian.
- Keep code, library names, and technical identifiers in their original language.
