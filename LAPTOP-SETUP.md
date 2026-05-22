# Laptop Setup

Follow these steps on the laptop after the desktop project has been pushed to a Git remote.

## 1. Check Git

Open PowerShell and run:

```powershell
git --version
```

If Git is missing, install it from:

https://git-scm.com/download/win

## 2. Configure Git Identity

Replace the values with your name and email:

```powershell
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## 3. Clone The Project

Choose a folder for Codex projects:

```powershell
mkdir $HOME\Documents\Codex
cd $HOME\Documents\Codex
git clone https://github.com/felixtan0902/codex-sync.git
```

## 4. Open In Codex

In Codex on the laptop:

- Sign in with the same ChatGPT account.
- Create or open a project using the cloned folder.
- Ask Codex: `Read CODEX-HANDOFF.md and continue from there.`

## Daily Flow

Before moving from desktop to laptop:

```powershell
git pull
git add .
git commit -m "work update"
git push
```

On the other device:

```powershell
git pull
```
