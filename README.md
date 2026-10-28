# Crash Bandicoot Double 2 — Windows preview v0.2.0

Download **CrashDouble2.exe**, open it on Windows 10/11 (64-bit), and choose your own original **Crash Bandicoot 2: Cortex Strikes Back USA / SCUS-94154 BIN**. The portable app includes the emulator and multiplayer integration. It does not include a game disc or BIOS, upload your BIN, or modify your original file.

- **Player-hosted rooms for up to five participants.** The host's PC coordinates the shared game state. Each player runs their own game locally. The public service handles room discovery, connection signalling and host leases.
- **Automatic host transfer.** If the host leaves, a participant with a current replica can take over. Among equally current copies, selection considers measured connectivity, latency, jitter and packet loss. A sudden loss requires the host lease to expire and can briefly pause synchronization.
- **Personal Wumpas remain personal.** Shared crate state and the existing cooperative modifications are retained.
- **Windows launcher with the pixel Crash life icon**, keyboard/controller support and microphone permission controls. The game viewport fits the window while keeping its 4:3 proportions. The joined-room counter uses the authoritative room state, including on guests.
- **The website is now a download page.** It does not start the emulator or poll the game APIs. Executable downloads are delivered through GitHub Releases.

The executable is not digitally signed. `SHA256SUMS.txt` is included so the downloaded file can be checked against this release.

## Playing together

Each player opens the app and loads their own compatible BIN. At Coco's camp, enter a player name and choose **Create Server** or **Search Server**. The host sets the limit to 2–5 players and selects **Start adventure** when everyone is ready. Enable the microphone only if you want voice chat.

## Validation and current scope

Two packaged Electron instances on the same PC joined one room, displayed both players together at Coco's camp, and entered the playing state. Closing the host window transferred that same room to the remaining player, who stayed in the game as the new host. This used real local WebRTC connections and a local directory service.

Automated tests exercised five desktop engines, shared facts, replica transfer, connection-based election, abrupt host loss, stale authority rejection, token recovery and cross-instance directory storage. These tests do **not** establish five independent players across the internet, all router/NAT configurations, or smooth performance on every PC. Direct connectivity or a configured TURN relay is still required. The complete cooperative campaign remains a work in progress.

This is an unofficial fan modification. Crash Bandicoot and the original game's code, characters, artwork, music and other assets belong to their respective rights holders. The download does not grant rights to the original game.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-bandicoot-2-online-brown.vercel.app/)
