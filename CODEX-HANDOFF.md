# Codex Handoff

Use this file to carry context between your desktop and laptop Codex sessions.

## Current Goal

- Sync this project between desktop and laptop.
- Keep project files in Git.
- Keep Codex chat context in this handoff file when moving devices.

## Desktop Status

- Git is installed.
- This folder is the desktop working copy for the sync project.
- GitHub CLI is not installed on this desktop.
- Git user name: `felixtan0902`.
- Git email: `92lix89@gmail.com`.
- GitHub repository: `https://github.com/felixtan0902/codex-sync`.
- Repository is initialized on `main` and tracks `origin/main`.
- Initial commit `13e05c8` (`Initial Codex sync setup`) is present in history.
- Latest commit `88eab78` (`Update Codex handoff status`) is present locally and on `origin/main`.
- Working tree is clean; there is no active rebase or merge conflict.

## Laptop Status

- Git was installed successfully on the laptop.
- The repository was cloned successfully to:

```text
C:\Users\PF2YQ\Documents\Codex\codex-sync
```

- Codex on the laptop can open that folder and continue by reading this file.

## Important Decision

- Codex chat history does not automatically sync between desktop and laptop.
- Project files sync through GitHub.
- Working context syncs through this `CODEX-HANDOFF.md` file.
- Before switching devices, update this file, commit, and push.
- On the other device, pull first, then ask Codex to read this file.

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

- On the laptop, run `git pull` before continuing work.
- Before switching devices again, update this handoff file with the latest status, commit, and push.
- Keep using GitHub as the shared project source.

## Daily Desktop/Laptop Commands

Before starting work on a device:

```powershell
git pull
```

Before switching to the other device:

```powershell
git add .
git commit -m "update handoff"
git push
```

