# Uhiva Launcher — Windows downloads

Official download page for **Uhiva Launcher**, the installer and updater for the **RoNCoopSquad** mod for
*Ready or Not*. This repository contains **only release downloads** — no source code.

➡️ **Download:** see [Releases](https://github.com/Adanirk/uhiva-launcher-releases/releases) and pick the newest
`Uhiva.Launcher_<version>_x64-setup.exe`.

> **Release candidate / pre-release.** The installer is **not code-signed** (no Authenticode certificate yet).
> Windows SmartScreen may say "Windows protected your PC — unknown publisher". Compare the SHA-256 listed in the
> release notes with the downloaded file (PowerShell: `Get-FileHash .\Uhiva.Launcher_0.2.0-rc.4_x64-setup.exe`)
> and only then choose *More info → Run anyway*. Do not disable Windows Defender or SmartScreen.

## How to install RoNCoopSquad with the launcher
1. Install **Ready or Not on Steam** and install **UE4SS** yourself (UE4SS is **not** included; the launcher never
   copies DLLs into the game).
2. Run the setup. It installs for your Windows user only (no administrator rights needed).
3. Start Uhiva Launcher → **Platforms → Rescan** → select your Steam installation.
4. The launcher checks for new releases at every start. Choose **0.4.2-alpha** → **Install** → check the folder
   shown in the confirmation, tick the box, confirm.
5. **Play via Steam**. Both co-op players need the **same** RoNCoopSquad version.

## What the launcher guarantees
- Mod packages come from the signed feed https://github.com/Adanirk/roncoopsquad-releases and are verified with the
  Uhiva publisher signature and SHA-256 before anything is written.
- Only the RoNCoopSquad folder and its entry in `mods.txt` / `mods.json` are changed. A full backup is made first;
  rollback, repair and uninstall are one click; nothing is written while the game is running.
- Old RoNCoopSquad builds that were not tested on the current game version are shown but blocked.

## Known limitations
- RoNCoopSquad 0.4.x is **alpha**. Please report every bug you find in our Discord: https://discord.gg/B3A8GrWg66
- Epic Games Store and Xbox PC: detected, but mod installation is not supported yet.
- Since **0.2.0-rc.4** the launcher checks for its own updates and for new RoNCoopSquad versions at every start and
  offers them; nothing is installed without your click. Launcher updates are verified with the Uhiva update
  signing key. **0.2.0-rc.3 and older cannot update themselves** — install rc.4 from this page once.
- No telemetry. The Statistics screen shows your own play time (stored only on your PC) and public GitHub
  download counters (downloads, not players).

Community: https://discord.gg/B3A8GrWg66 · Unofficial fan-made software, not affiliated with or endorsed by
VOID Interactive.
