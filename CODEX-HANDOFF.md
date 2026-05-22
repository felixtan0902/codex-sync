# Codex Handoff

Use this file to carry context between your desktop and laptop Codex sessions.

## Current Goal

- Sync this project between desktop and laptop.
- Keep project files in Git.
- Keep Codex chat context in this handoff file when moving devices.

## Desktop Status

- Git is installed.
- This folder has been prepared as the sync project folder.
- GitHub CLI is not installed on this desktop.
- Git user name: `felixtan0902`.
- Git email: `92lix89@gmail.com`.
- GitHub repository: `https://github.com/felixtan0902/codex-sync`.
- Codex prepared the files, but the final Git commit/push must be run from normal PowerShell because the Codex sandbox cannot write Git lock files in `.git`.

## How To Hand Off Before Switching Devices

Ask Codex:

> Update `CODEX-HANDOFF.md` with the current status, files changed, decisions made, open questions, and next steps.

Then commit and push:

```powershell
git add .
git commit -m "update Codex handoff"
git push
```

## How To Continue On The Other Device

After pulling the latest project files, ask Codex:

> Read `CODEX-HANDOFF.md` and continue from there.

## Next Steps

- Run the desktop commands from normal PowerShell.
- Clone that repository on the laptop.

## Desktop Commands

Run these from normal PowerShell:

```powershell
cd "C:\Users\User\Documents\Codex\2026-05-22\saya-punya-codex-di-desktop-ini"
git config user.name "felixtan0902"
git config user.email "92lix89@gmail.com"
git add .
git commit -m "Initial Codex sync setup"
git remote add origin https://github.com/felixtan0902/codex-sync.git
git push -u origin main
```
