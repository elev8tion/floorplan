# Floorplan project instructions

This fork is maintained with Pi. Use the project-local `floorplan` skill in `.agents/skills/floorplan/SKILL.md` whenever creating or updating a codebase map, answering a question from a map, or planning a system blueprint. That skill replaces the Claude Code session workflow for Pi; do not require Claude Code to perform these tasks.

## Codebase context

- This repository is indexed by vnodes. For coding tasks, orient with one vnodes pipeline call, check the impact graph before editing, save a durable observation for kept changes, then run `vnodes index` and `vnodes check`.
- The implementation and its tests live under `skills/floorplan/` and `tests/`. The product intentionally supports Claude Code and Codex as external integrations; do not remove or break those compatibility paths while working on the Pi-local workflow unless explicitly requested.
- Run `npm test` for code changes. For changes to skill/docs only, validate the skill is discoverable in Pi and keep the vnodes index current.
