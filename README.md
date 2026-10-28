# Crash Bandicoot Double 2 — Windows preview v0.3.0

Download **CrashDouble2.exe**, open it on Windows 10/11 (64-bit), and choose your own original **Crash Bandicoot 2: Cortex Strikes Back USA / SCUS-94154 BIN**. The portable app includes the emulator and multiplayer integration. It does not include a game disc or BIOS, upload your BIN, or modify your original file.

This version moves room discovery and coordination to Cloudflare. **All participants must update to 0.3.0**: previous versions use the old directory and cannot see these new rooms.

- **Five participants per room**, including the host. Each player runs the game locally; game state and replicas travel between participants.
- **WebSocket room updates** replace recurring HTTP synchronization. Outside a room, the app makes no periodic room-directory requests. Open Search Server or press Refresh to find rooms.
- **Separate SQLite storage for each room** through Cloudflare Durable Objects. Routine presence updates do not rewrite the database of all rooms. Inactive rooms expire and disappear from discovery.
- **Automatic host transfer** retains the most recent replica and considers connection quality among equally current candidates. A sudden host disconnect may pause synchronization until the 18-second host lease expires.
- **Personal Wumpas remain personal.** The existing crate and cooperative game behavior is retained.

The website is a static download and instructions page; downloads come from GitHub Releases. No Supabase credentials or Cloudflare account credentials are embedded in the app.

## Playing together

Each player opens the updated app and loads their own compatible BIN. At Coco's camp, enter a name and choose **Create Server** or **Search Server**. The host sets the limit to 2–5 players and selects **Start adventure** when everyone is ready. Enable the microphone only if you want voice chat.

The executable is not digitally signed. `SHA256SUMS.txt` identifies the released file.

## Scope

The complete cooperative campaign remains a work in progress. Direct WebRTC connectivity or a configured TURN relay is required; this migration does not guarantee connectivity through every router, NAT or carrier network.

This is an unofficial fan modification. Crash Bandicoot and the original game's code, characters, artwork, music and other assets belong to their respective rights holders. The download does not grant rights to the original game.

## Validation before release

The packaged 0.3.0 executable was tested with two independent emulator windows on one Windows PC against the public Cloudflare service: both players joined Coco's camp, appeared together, started the same adventure, and the guest became host in the same ongoing room after the original host window closed. This is not a test across two household networks or five simultaneous emulators.

Five controlled clients also passed capacity, reconnect, stale-host rejection, and graceful/abrupt host migration checks. Existing game/server regression tests passed 336/336; desktop transport tests passed 23/23; Worker tests passed 13/13.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-double-2-directory.gabrielcavalcanteoficial.workers.dev/)
