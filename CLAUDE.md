## Building with Codex

This project is built with help from the `codex-headless` plugin. Claude scopes the work and checks the results, and Codex helps along the way:

- `codex-headless:exec` hands implementation work to Codex (`codex exec`) to write the code.
- `codex-headless:advise` gets a second opinion from Codex and Fable, once before settling on an approach and once before calling work done.

## Agent skills

### Issue tracker

Issues live in GitHub Issues for GauranshMathur/hunterr, accessed with the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Uses the five default labels: needs-triage, needs-info, ready-for-agent, ready-for-human, wontfix. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one root `GLOSSARY.md` plus `docs/adr/`, both created only when needed. See `docs/agents/domain.md`.
