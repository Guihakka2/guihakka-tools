# Guihakka Tools

Small, privacy-first, open-source tools for developers and everyday users. Local by default, no telemetry.

Each tool lives in its own repository. English first; Portuguese (pt-BR) and Japanese (ja) docs follow once a tool is stable.

## Released

| Tool | What it does | Install |
|---|---|---|
| [envdiff](https://github.com/Guihakka2/envdiff) | Compare `.env` files across environments without printing secrets | `npx @guihakka/envdiff` |

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

### Desktop & everyday
| # | Tool | Problem | Status |
|---|---|---|---|
| 15 | ClipClean | Fix broken line breaks/spacing in text copied from PDFs | 💡 |
| 16 | DropSort | Auto-organize files with preview and undo | 💡 |
| 17 | ScreenshotFinder | Search screenshots by the text inside them (local OCR) | 💡 |
| 18 | MeetingReady | One-click mic/camera/speaker/network check | 💡 |
| 19 | FormEasy | Fill PDF forms from saved local profiles | 💡 |
| 20 | CancelRadar | Track subscriptions and free-trial end dates | 💡 |
| 21 | PageDiff | Watch web pages for changes | 💡 |
| 22 | LifeTranslate | Translate documents into a to-do list with deadlines | 💡 |
| 23 | UseFirst | Home food/product inventory with expiry reminders | 💡 |
| 24 | ReplyLater | Reminders for messages you need to answer | 💡 |
| 25 | DownloadDoctor | Broken downloads, corrupt ZIPs, duplicates, checksums | 💡 |
| 26 | ReceiptBox | Extract date/amount/store from receipts to CSV | 💡 |
| 27 | LinkKeeper | Saved links with broken-link detection | 💡 |
| 28 | SimpleTransfer | Encrypted file transfer on the same Wi-Fi, QR pairing | 💡 |
| 29 | TimeZoneMate | Meeting times across time zones and holidays | 💡 |

## Principles

1. **Local first** — no data leaves your machine unless the tool's job requires it.
2. **Minimal dependencies** — every dependency is attack surface.
3. **Signed releases** — published from CI with provenance, never by hand.
4. **Validate before building** — a tool moves from 💡 to 🚧 only when people ask for it.

## License

MIT
