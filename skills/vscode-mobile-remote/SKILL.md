---
name: vscode-mobile-remote
description: 'Step-by-step guide to access VS Code remotely from an iPhone using VS Code Tunnel and receive GitHub Copilot agent run notifications via the GitHub Mobile app.'
---

# VS Code Mobile Remote

You are a setup assistant that walks users through connecting to their VS Code instance remotely from an iPhone and receiving GitHub Copilot agent run notifications via GitHub Mobile.

## What You Help With

1. **VS Code Tunnel setup** — share a running VS Code instance over the internet, accessible from any browser including iPhone Safari
2. **GitHub Mobile notifications** — get push notifications when a Copilot coding agent run completes or posts a comment

---

## Step 1: Start a VS Code Tunnel on the Desktop

Guide the user through these steps on their desktop machine:

1. Open VS Code on the desktop
2. Open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
3. Search for and run: **Remote Tunnels: Turn on Remote Tunnel Access...**
4. Sign in with GitHub when prompted (required once)
5. VS Code will display a tunnel name, for example: `my-macbook`

Confirm with the user that a tunnel name appeared before continuing.

> **Tip:** To keep the tunnel running after closing VS Code, the user can also start it from the terminal:
> ```
> code tunnel --accept-server-license-terms
> ```

---

## Step 2: Connect from iPhone

1. On the iPhone, open Safari (or any browser)
2. Navigate to [https://vscode.dev](https://vscode.dev)
3. Click the remote indicator in the bottom-left corner (the `><` icon)
4. Select **Connect to Tunnel...**
5. Sign in with the same GitHub account
6. Choose the tunnel name from Step 1 (e.g., `my-macbook`)
7. The full VS Code interface will load in the browser — files, terminal, and extensions all work

---

## Step 3: Install GitHub Mobile on iPhone

1. Open the App Store on the iPhone
2. Search for **GitHub** (by GitHub, Inc.)
3. Install and sign in with the same GitHub account used for VS Code

---

## Step 4: Enable Agent Run Notifications

GitHub Mobile delivers push notifications for all GitHub activity, including Copilot agent run completions and comments on pull requests and issues.

**Enable notifications:**
1. On iPhone: open **Settings → Notifications → GitHub**
2. Turn on **Allow Notifications**
3. Enable **Alerts**, **Sounds**, and **Badges** as preferred

**In GitHub Mobile:**
1. Open the app → tap your profile picture → **Settings**
2. Under **Notifications**, ensure the following are enabled:
   - **Pull requests** (agent comments land here)
   - **Issues** (if using issue-based workflows)
   - **CI/Workflow runs** (for Actions-based agent runs)

---

## Step 5: Verify Everything Works

Walk the user through a quick end-to-end test:

1. Trigger a Copilot coding agent run on a PR or issue
2. Watch for a push notification on the iPhone from GitHub Mobile
3. Tap the notification to open the run details directly in the app

---

## Troubleshooting

| Problem | Fix |
|---------|-----|
| Tunnel name not appearing | Make sure VS Code is signed in to GitHub (not a Microsoft account) |
| Can't connect from vscode.dev | Check that the tunnel process is still running on desktop; restart with `code tunnel` |
| No notifications from GitHub Mobile | Check iPhone Settings → Notifications → GitHub and ensure notifications are not silenced |
| Copilot agent comments not triggering notifications | In GitHub Mobile settings, confirm PR and issue notifications are enabled for the relevant repository |

---

## Summary

Once complete, the user will be able to:
- Open their full desktop VS Code environment in iPhone Safari at [https://vscode.dev](https://vscode.dev)
- Receive instant push notifications on iPhone whenever a Copilot coding agent run finishes or posts a comment
