# Crash Double 2 for Windows · 0.3.2

Shared box synchronization now detects crate-state changes every frame and
immediately requests a validated native observation when needed, rather than
missing short-lived boxes between the 100 ms fallback samples. Boxes broken by
one player can disappear and count for the other while both remain in the level.
Wumpas stay personal to the player who broke the box.

Delivered jewels now use the original game's permanent inventory and native
warp-room objects. An observer who stays in the warp can see the delivered gem
in its original position, shape and size without entering another level first.
The permanent substitute image is suppressed when the native objects are active.
The collector's original delivery sequence and shared ownership rules remain.

A short expiration of a collectible reservation no longer discards an already
observed native pickup. The client can renew its reservation and finish that
pickup when the item is still available. A changed owner, new item generation,
level/session change, rewind or long observation gap cancels recovery, so stale
state cannot grant a jewel or override another player's ownership.

The release keeps **up to 5 players**, Cloudflare room discovery over WebSockets,
player-hosted matches and automatic host migration. Use 0.3.2 on all participating
PCs to receive these fixes. Restart the game normally with your original disc;
an old emulator save state may retain objects from the older patch.

Download `CrashDouble2.exe` and open it on Windows 10 or 11 (64-bit). Select
your own original **Crash Bandicoot 2: Cortex Strikes Back USA / SCUS-94154 BIN**.
No game disc, ROM, BIOS, save file, account credential or private database backup
is included. The application is currently unsigned. Verify the executable
against the accompanying `SHA256SUMS.txt`.

Two actual emulator sessions verified a normal Turtle Woods box break: both
counters reached 1, the box was removed remotely, and Wumpas remained personal.
A Turtle Woods bonus test then shared five bonus boxes with the player outside
the bonus. Together with the normal box and one crate originating as a checkpoint, both
players had a total of 7 after the bonus exit; the temporary bonus count cleared
without losing or counting those boxes twice.
A separate live route verified a blue-gem collection, native end-platform
return and original delivery, while the other player remained in the warp.
The same observer-side native object became visible at its original location;
no permanent replacement sprite or warp reload was used.

Other gem and crystal variants have focused code and ownership regression
coverage. The reservation-recovery regression was reproduced using captured
native RAM and the real inventory controller and passed its affected automated
tests; it has not been separately approved in a real gameplay run after the fix.
This round did not complete every level, all bonus boxes, every jewel
or a five-emulator campaign. The complete cooperative campaign remains a work
in progress. Direct WebRTC connectivity or a configured TURN relay is required;
connectivity through every router or carrier network is not guaranteed.

The Windows package passed 23 desktop tests. Its bundled runtime matches the
reviewed source; the package audit checked excluded media and credentials,
security settings and all seven logo-icon sizes in both Windows executables.

This is an unofficial fan project. Crash Bandicoot and associated characters,
names and game assets belong to their respective rights holders. This project
is not affiliated with or endorsed by those rights holders.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-double-2-directory.gabrielcavalcanteoficial.workers.dev/)
