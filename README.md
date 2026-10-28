# Crash Double 2 for Windows · 0.3.1

The portable Windows application now uses the full Crash Double 2 website logo for its executable and window icons. The logo keeps its proportions and transparency at the icon sizes supported by Windows.

This is a visual update to 0.3.0. Rooms still use Cloudflare WebSockets, with up to **5 players**, automatic host migration, and personal Wumpa fruit. The host runs the match simulation. No gameplay rules or network protocol were changed for this icon update.

Download `CrashDouble2.exe` and open it on Windows 10 or 11 (64-bit). Select your own original **Crash Bandicoot 2: Cortex Strikes Back USA / SCUS-94154 BIN** in the application. No game disc, ROM, BIOS, save file, account credential, or private database backup is included in the download. The application is currently unsigned.

At Coco's camp, enter a name and choose **Create Server** or **Search Server**. The host chooses 2–5 players and selects **Start adventure** when everyone is ready. Participants need version 0.3.0 or newer for the Cloudflare room directory.

The complete cooperative campaign remains a work in progress. Direct WebRTC connectivity or a configured TURN relay is required; connectivity through every router, NAT, or carrier network is not guaranteed. A sudden host disconnect can pause synchronization until the 18-second host lease expires.

This is an unofficial fan project. Crash Bandicoot and associated characters, names and game assets belong to their respective rights holders. This project is not affiliated with or endorsed by those rights holders.

SHA-256 for the portable executable is provided in `SHA256SUMS.txt` beside this download. Keep your previous version until you confirm the new one opens correctly on your PC.

Validation for this update: 23 desktop tests and 14 export tests passed; the packaged application opened on Windows with the new window icon. All seven icon sizes were verified inside both the portable launcher and the runtime executable. Packaged runtime files were checked against the source. This visual update did not repeat the previous release's two-emulator multiplayer test.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-double-2-directory.gabrielcavalcanteoficial.workers.dev/)
