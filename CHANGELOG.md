# Changelog

All notable changes to this project will be documented in this file.

## 0.1.3 - 2026-03-28

### Fixed

- Added top-level skill alias links (`sprint-task`, `sprint-board`, `sprint-finish`) during install so Claude/Conductor environments that scan one level of `~/.{codex|claude}/skills` can discover them.

## 0.1.2 - 2026-03-28

### Added

- Added standalone Conductor-visible skills: `sprint-task`, `sprint-board`, `sprint-finish`.
- Installer now deploys those skill manifests under the sprint package install root.

## 0.1.1 - 2026-03-28

### Fixed

- Codex install target now uses `~/.codex/prompts` for slash commands instead of `~/.codex/commands`.
- Added YAML frontmatter to `commands/sprint*.md` files so Codex recognizes them as custom prompts.
- Updated README verification examples to use the Codex prompts directory.

## 0.1.0 - 2026-03-28

Initial release.

### Added

- `sprint` skill package for multi-agent sprint coordination in Conductor.
- Helper scripts: `sprint-setup`, `sprint-board`, and `sprint-finish`.
- Slash command docs: `/sprint`, `/sprint-task`, `/sprint-board`, and `/sprint-finish`.
- Host-aware installer support for Codex and Claude install paths.
