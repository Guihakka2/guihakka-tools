# Guihakka Tools

Small, privacy-first, open-source tools for developers and everyday users. Local by default, no telemetry.

Each tool lives in its own repository: zero runtime dependencies, tested on Linux, macOS and Windows, releases published from CI with provenance. Docs in English, Portuguese (pt-BR) and Japanese (ja).

## Tools

| Tool | What it does | Install |
|---|---|---|
| [envdiff](https://github.com/Guihakka2/envdiff) | Compare `.env` files across environments without printing secrets | `npx @guihakka2/envdiff` or [download the program](https://github.com/Guihakka2/envdiff/releases/latest) ¹ |
| [logclump](https://github.com/Guihakka2/logclump) | Group similar errors in huge log files, with first and last seen times | `npx @guihakka2/logclump` or [download the program](https://github.com/Guihakka2/logclump/releases/latest) ¹ |
| [apishape](https://github.com/Guihakka2/apishape) | Catch breaking JSON API changes in CI; snapshots hold no values | `npx @guihakka2/apishape` or [download the program](https://github.com/Guihakka2/apishape/releases/latest) ¹ |
| [tlsdue](https://github.com/Guihakka2/tlsdue) | TLS certificate and domain expiry checks, free monitoring on GitHub Actions | `npx @guihakka2/tlsdue` or [download the program](https://github.com/Guihakka2/tlsdue/releases/latest) ¹ |
| [whohasaccess](https://github.com/Guihakka2/whohasaccess) | Read-only audit of who and what can access your GitHub repositories | `npx @guihakka2/whohasaccess` or [download the program](https://github.com/Guihakka2/whohasaccess/releases/latest) ¹ |
| [dumpproof](https://github.com/Guihakka2/dumpproof) | Prove a Postgres/MySQL/SQLite backup restores, in an offline throwaway container | `npx @guihakka2/dumpproof` or [download the program](https://github.com/Guihakka2/dumpproof/releases/latest) ¹ |
| [downloaddoctor](https://github.com/Guihakka2/downloaddoctor) | Find broken downloads: truncated files, corrupt zips, checksum mismatches | `npx @guihakka2/downloaddoctor` or [download the program](https://github.com/Guihakka2/downloaddoctor/releases/latest) ¹ |
| ai-guard-lock | (existing project) | |

¹ **No Node.js needed**: every tool also has standalone programs for Windows (x64, ARM), macOS (Apple silicon, Intel) and Linux (x64, ARM), built by GitHub Actions with a `SHA256SUMS.txt` and a build provenance attestation. Not code-signed with a paid certificate yet, so the first run shows a SmartScreen or Gatekeeper warning; the tool's README explains how to allow it.

**For AI agents**: envdiff, logclump and whohasaccess also run as read-only [MCP](https://modelcontextprotocol.io) servers (`--mcp`), so coding agents like Claude Code, Codex or Cursor can use them without ever seeing secret values.

## Ideas we did not build, and why

Before building, every idea is checked against existing projects. If a good open-source tool already does the job, we point to it instead of making a copy.

| Idea | Use this instead |
|---|---|
| PRGuardian: PRs and CI across many repos | [gh-dash](https://github.com/dlvhdr/gh-dash) |
| UpdateRisk: risks before upgrading dependencies | [npm-check-updates](https://github.com/raineorshine/npm-check-updates) + [Renovate](https://github.com/renovatebot/renovate) + `npm audit` |
| CronProof: alert when cron jobs don't run | [healthchecks](https://github.com/healthchecks/healthchecks) |
| DiskDetective: dev caches eating disk | [npkill](https://github.com/voidcosmos/npkill), [kondo](https://github.com/tbillington/kondo) |
| NetPulse: new devices on your network | [NetAlertX](https://github.com/netalertx/NetAlertX), [WatchYourLAN](https://github.com/aceberg/WatchYourLAN) |
| CloudWaste: idle cloud resources | [Komiser](https://github.com/mlabouardy/komiser) |
| MicGuard: mic/camera activity | [OverSight](https://github.com/objective-see/OverSight) (macOS), Windows privacy indicators |
| SimpleTransfer: file transfer on the same Wi-Fi | [LocalSend](https://github.com/localsend/localsend) |

## Principles

1. **Local first**: no data leaves your machine unless the tool's job requires it.
2. **Zero runtime dependencies**: every dependency is attack surface.
3. **Signed releases**: published from CI with provenance, never by hand.
4. **No copies**: build only what doesn't already exist in a good form.

## License

MIT
