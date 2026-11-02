# Crash Double 2 for Windows · 0.3.3

You can now open `CrashDouble2.exe` more than once on the same PC. Each launch
opens an independent player window with its own temporary session, local server
and Chromium profile. A short session label identifies each window.

The portable launcher also extracts to a different directory for each launch.
Closing one copy no longer risks removing files used by another copy. The
application still allows time for automatic host migration before exiting.

To test two players, open the new executable twice, select your own original
USA SCUS-94154 BIN in each window and enter different player names. Create a
server in the first window and join it from the second. Once both have arrived
at Coco's camp, the host can start the adventure. Keyboard/controller input
goes to the focused window; switch windows to control the other player.

Normal sessions are temporary and do not reuse the previous window's login,
room membership or browser storage. Your original game file is not modified.
Existing explicit QA profiles remain supported for development tests.

Validation: 30 desktop tests and 14 public-export tests passed. Two ordinary
portable launches, without QA flags, ran simultaneously and joined the same
five-player room as two distinct players. Closing the first window left the
second running and transferred room hosting to it. A third ordinary launch
then opened independently while that second window remained active. The package
audit confirmed source consistency, private-file exclusion and security settings.
This release's acceptance covered the launcher, lobby and host handoff; it did
not repeat a full in-level gameplay session or the previous crate/gem playthroughs.

This release preserves the 0.3.2 cooperative fixes, personal Wumpas, the
five-player room limit, Cloudflare discovery and automatic host migration.
It does not change gameplay rules or increase the room capacity.

No disc, ROM, BIOS, personal save, account credential or private database
backup is included. Every player supplies their own compatible original game.

This is an unofficial fan project. Crash Bandicoot and associated characters,
names and game assets belong to their respective rights holders. This project
is not affiliated with or endorsed by those rights holders.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-double-2-directory.gabrielcavalcanteoficial.workers.dev/)
