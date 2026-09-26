# Template

Template is the canonical repository scaffold for portable JLS skills. It preserves the shared release, versioning, test-build, installation-documentation, and licensing conventions used across JLS skill repositories.

Skills built from Template support OpenAI Codex and Claude Code.

## Use

Copy this repository for a new portable skill, then replace the template metadata and skill content. Keep the shared workflow structure intact unless the skill's packaging or runtime requirements genuinely require a different build path.

The workflow scaffold separates reusable Build, manual Test, scheduled Nightly, manual Release, and automatic Test Trigger concerns. Release derives major/minor/patch versions from the current stable release or can replace the current release; source `manifest.json` does not track a version. Creating an ephemeral `jls-test/**` branch dispatches Test and the trigger workflow deletes that branch automatically.

## Install

Template itself is a development scaffold and is not intended for installation as an end-user skill.

## License

This project is licensed under the [MIT License](LICENSE). Copyright © 2026 Jacob Lockett.
