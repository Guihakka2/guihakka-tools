# Guihakka Tools

Small, privacy-first, open-source tools for developers and everyday users. Local by default, no telemetry.

Each tool lives in its own repository. English first; Portuguese (pt-BR) and Japanese (ja) docs follow once a tool is stable.

## Released

| Tool | What it does | Install |
|---|---|---|
| [envdiff](https://github.com/Guihakka2/envdiff) | Compare `.env` files across environments without printing secrets | `npx @guihakka2/envdiff` |

## Idea backlog

Status: 💡 idea · 🔍 validating demand · 🚧 building · ✅ released.
Have the problem one of these solves? 👍 or comment on its issue — that decides what gets built next.

### Developer tools
| # | Tool | Problem | Status |
|---|---|---|---|
| 1 | EnvDiff | `.env` drift between dev/staging/prod | ✅ |
| 2 | PRGuardian | PRs, reviews and CI failures across many repos in one view | 💡 |
| 3 | LogLens | Group similar errors in huge log files, first-seen time | 💡 |
| 4 | APISnapshot | Detect unintended JSON API response changes in CI | 💡 |
| 5 | UpdateRisk | Breaking changes + CVEs before upgrading dependencies | 💡 |
| 6 | CronProof | Alert when scheduled jobs don't run or get slow | 💡 |
| 7 | DiskDetective | Find dev caches, Docker images and old logs eating disk | 💡 |

### Security & infrastructure
| # | Tool | Problem | Status |
|---|---|---|---|
| 8 | DockerRescue | Back up Docker volumes/DBs and verify restores work | 💡 |
| 9 | CertWatch | SSL certificate and domain expiry monitoring | 💡 |
| 10 | NetPulse | Notify on new devices / IP changes on your own network | 💡 |
| 11 | AccessMap | Leftover and excessive permissions in GitHub/cloud | 💡 |
| 12 | CloudWaste | Idle resources and cost spikes in AWS (read-only) | 💡 |
| 13 | MicGuard | See when mic/camera are active | 💡 |
| 14 | ai-guard-lock | (existing project) | ✅ |

### Desktop & privacy
| # | Tool | Problem | Status |
|---|---|---|---|
| 15 | DownloadDoctor | Broken downloads, corrupt ZIPs, duplicates, checksums | 💡 |
| 16 | SimpleTransfer | Encrypted file transfer on the same Wi-Fi, QR pairing | 💡 |

## Principles

1. **Local first** — no data leaves your machine unless the tool's job requires it.
2. **Minimal dependencies** — every dependency is attack surface.
3. **Signed releases** — published from CI with provenance, never by hand.
4. **Validate before building** — a tool moves from 💡 to 🚧 only when people ask for it.

## License

MIT
