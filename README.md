# Crash Double 2 for Windows · 0.3.4

Online Options is now available from the game's Start menu, above the original
Options entry. The menu contains Resume, Online Options, Options and Quit.
Options retains the original game settings; the new online submenu uses the
native interface font with orange lettering and a stone-colored frame.

During the adventure, press Start on your controller or Enter on the keyboard,
then choose Online Options to manage your current room. Returning from the
online submenu brings you back to the Start menu. Coco's waiting area keeps
its Search Server and Create Server entries for the initial connection.

Quit leaves your current server and returns you to Coco's waiting area using
the disc already loaded in the app. You do not need to select your original BIN
again. Other players stay in their adventure; if the departing player was the
host, the existing host migration transfers the room to a remaining player.

This release keeps the five-player limit, personal Wumpas, Cloudflare room
discovery and automatic host migration. Multiple independent player windows
on the same PC remain supported.

The Start menu no longer draws remote players and name labels over its panels.
Menu resource checks now use bounded reads instead of copying the whole resource
on every frame. A guarded return also preserves the original calibration flow.

Validation: 357 online tests, 30 desktop tests and 15 native-menu tests passed.
Two real player windows joined and started together; Online Options and Back to
Start were checked visually. The user confirmed normal original Options/Sound
controls, then Quit returning to Coco without selecting the BIN again while the
other player continued. The surviving session was also observed with one player
and the adventure still running. These checks cover the menu and lobby flow;
they are not a new complete-level or five-player performance acceptance.
The final Windows package was audited against the current source, including
the website-logo icon. No source drift, private files or credentials were found.

No disc, ROM, BIOS, personal save, account credential or private database
backup is included. Every player supplies their own compatible original USA
SCUS-94154 game. The app patches a temporary local copy and does not modify the
original file.

This is an unofficial fan project. Crash Bandicoot and associated characters,
names and game assets belong to their respective rights holders. This project
is not affiliated with or endorsed by those rights holders.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-double-2-directory.gabrielcavalcanteoficial.workers.dev/)
