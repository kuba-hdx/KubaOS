<div align="center">

# KubaOS

**The local-first founder OS.**

A private, offline desktop cockpit for a solo founder — interviews, pains, features,
build logs, metrics, launch tasks, content calendar, and focus mode, all in one place.

[Download KubaOS 0.1.2 (Windows MSI)](https://github.com/kuba-hdx/KubaOS/releases/latest) · [Showcase on kuba-hdx.dev](https://kuba-hdx.dev/KubaOS) ·
[Virustotal Scan](https://www.virustotal.com/gui/file/5e7da9a1b0d788bf325124e179332f621b34de38f3ad696bd47d9cc8a18d2d9b)
</div>

---

## What it is

KubaOS is a single-user, local-first productivity environment built for founders who
want their operating picture in one place without shipping it to a third party.
Your data lives on your machine. The app only reaches out for optional cloud sync,
update checks, and integrations you explicitly configure.

## What it does

- **Interviews & pains** — capture customer conversations, extract pains, link them
  to features you ship.
- **Build log** — structured timeline of what you shipped, when, and why.
- **Metrics & launch tasks** — track the numbers that matter and the work that moves them.
- **Content calendar** — plan posts, videos, and shipping moments alongside the build.
- **Today / focus mode** — a zero-distraction view of the one thing that matters today.
- **Forum** — private async thread stream for side conversations with collaborators.
- **Auto-updates** — every new release installs silently in the background.

## Stack

- **Shell** — Tauri 2 (Rust) + WiX MSI bundler
- **UI** — Next.js 15, React 19, Tailwind CSS 4, Radix, Framer Motion
- **Storage** — local SQLite (rusqlite), OS keychain for secrets
- **Sync** — Supabase (optional, per-user)

## Security

- Signed MSI installer
- Strict CSP, no remote scripts, no remote styles
- Context menus, devtools hotkeys, and save-page disabled in production
- Secrets stored in the Windows Credential Manager (not in plaintext)
- Session tokens are not persisted to disk

## Install

1. Download the latest MSI from the [releases page](https://github.com/kuba-hdx/KubaOS/releases/latest).
2. Run the installer.
3. Launch **KubaOS** from the Start menu.
4. Sign in or create a local account. The onboarding tour runs automatically on first launch.

Updates install silently — no manual action required.

## Status

KubaOS is a personal tool built by [Kuba (hdx)](https://kuba-hdx.dev) and published as
a closed-source binary. This repository hosts the download, release notes, and visual
showcase only — the source is not public.

## License

© Kuba. All rights reserved.
