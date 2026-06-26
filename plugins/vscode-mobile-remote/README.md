# VS Code Mobile Remote

Remote control VS Code from your iPhone and get push notifications for Copilot agent runs — using VS Code Tunnel and GitHub Mobile.

## Who Is This For?

Anyone who wants to:
- Access their desktop VS Code environment from an iPhone (or any mobile browser)
- Receive instant push notifications when a GitHub Copilot coding agent run completes or posts a comment

No third-party apps, no SSH setup, no monthly subscriptions — just VS Code, a GitHub account, and the free GitHub Mobile app.

## Installation

```bash
copilot plugin install vscode-mobile-remote@awesome-copilot
```

## Getting Started

```
use vscode-mobile-remote
```

The skill walks you through five steps:

1. **Start a VS Code Tunnel** on your desktop machine
2. **Connect from iPhone Safari** at [https://vscode.dev](https://vscode.dev)
3. **Install GitHub Mobile** on your iPhone
4. **Enable Copilot agent notifications** in GitHub Mobile and iPhone Settings
5. **Verify** with a quick end-to-end test

## What's Included

| Skill | What It Does |
|-------|-------------|
| `vscode-mobile-remote` | Interactive setup guide with troubleshooting for VS Code Tunnel + GitHub Mobile notifications |

## Requirements

| Requirement | Details |
|-------------|---------|
| VS Code | Latest stable release on your desktop |
| GitHub account | Same account on desktop VS Code and iPhone |
| iPhone | Safari browser (iOS 14+) |
| GitHub Mobile app | Free, available on the App Store |

## Features

| Feature | Description |
|---------|-------------|
| **Full VS Code in Safari** | Files, terminal, extensions — the complete IDE in your iPhone browser |
| **Push notifications** | Instant alerts when Copilot agent runs complete or comment on PRs/issues |
| **No extra infrastructure** | Uses built-in VS Code Tunnel — no self-hosted server needed |
| **Troubleshooting guide** | Common problems and fixes included |

## How It Works

VS Code Tunnel creates a secure, authenticated connection between your desktop VS Code and [vscode.dev](https://vscode.dev). GitHub Mobile connects to your GitHub account and delivers push notifications for any activity — including Copilot coding agent run completions, PR comments, and workflow status updates.

Together, they give you full remote development capabilities and real-time agent monitoring on any iPhone.

## Source

This plugin is part of [Awesome Copilot](https://github.com/github/awesome-copilot), a community-driven collection of GitHub Copilot extensions.

## License

MIT
