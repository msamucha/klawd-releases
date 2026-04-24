# Klawd — Desktop App

Download installers for the Klawd desktop app.

→ **[Download latest release](https://github.com/msamucha/klawd-releases/releases/latest)**

## Install on Mac

1. Download the `.dmg` matching your Mac:
   - **Apple Silicon** (M1, M2, M3, M4): `Klawd-x.y.z-arm64.dmg`
   - **Intel Mac**: `Klawd-x.y.z.dmg` (coming soon)
2. Open the DMG, drag **Klawd.app** into the Applications folder
3. Run this command in Terminal **once** to bypass Gatekeeper:

   ```sh
   xattr -dr com.apple.quarantine /Applications/Klawd.app
   ```
4. Double-click Klawd in Applications. The app opens normally from now on.

## Why the Terminal step?

Klawd is not yet signed with an Apple Developer certificate. macOS's
Gatekeeper marks unsigned apps downloaded from the web as "damaged"
and refuses to open them — even with the right-click → Open trick that
worked in older macOS versions.

The `xattr` command above removes the quarantine flag Safari/Chrome
attached to the file. macOS then trusts the local copy. You only need
to run this once per installed version.

When we eventually pay for an Apple Developer certificate ($99/year)
and notarize the app, this step goes away. Until then it's the price
of admission.

## Login

In the desktop app, log in with **email + password**. Magic-link
emails redirect to your browser, not back to the app, so they don't
end up logging you in inside Klawd.

If you don't have a password set yet, ask Michel to set one for you
(via Supabase Dashboard).

## What's in this repo

Just release artifacts. Source code lives in private repos. No code
or contributions land here.

## Issues / feedback

Write to **hello@klawd.app**.
