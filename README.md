# Klawd — Desktop App

Download installers for the Klawd desktop app.

→ **[Download latest release](https://github.com/msamucha/klawd-releases/releases/latest)**

## Install on Mac

1. Download the `.dmg` matching your Mac:
   - **Apple Silicon** (M1, M2, M3, M4): `Klawd-x.y.z-arm64.dmg`
   - **Intel Mac**: `Klawd-x.y.z.dmg` (coming soon)
2. Open the DMG, drag **Klawd.app** into Applications
3. **Right-click** Klawd in Applications → **Open** → **Open Anyway**

The app is not code-signed yet, so macOS Gatekeeper will refuse to open it on first launch with double-click. The right-click → Open dance is needed once per installed version. After that, double-click works normally.

## Login

In the desktop app, use **email + password**. Magic-link login redirects to the browser instead of back to the app — you can still trigger it from the toggle, but the session won't end up in the app. We're working on a proper desktop auth flow.

If you don't have a password set yet, ask Michel to set one for you (Supabase Dashboard).

## What's in this repo

Just release artifacts. Source code lives in private repos. No code or contributions go here.

## Issues

For bug reports / feedback, write to **hello@klawd.app**.
