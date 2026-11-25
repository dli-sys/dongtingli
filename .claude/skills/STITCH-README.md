# Stitch skills

Copied from https://github.com/google-labs-code/stitch-skills (commit 75f4696),
the `stitch-design` and `stitch-utilities` plugins. Licensed under Apache 2.0,
see `STITCH-LICENSE`.

Only change from upstream: skills named `stitch::<name>` were renamed to
`stitch-<name>` (folder and `name:` field), because Claude Code skill names
may only use lowercase letters, numbers and hyphens.

Most of these skills call the Google Stitch MCP server, which has to be
connected with a Stitch API key (https://stitch.withgoogle.com/docs/mcp/setup/).
`enhance-prompt`, `site-md` and `stitch-extract-design-md` work without it.

To update, re-copy the two plugins' `skills/` folders from upstream and redo the rename.
