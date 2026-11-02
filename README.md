# Crash Double 2 for Windows · 0.3.5

Coco's waiting area now uses the same Online Options interface as the game's
Start menu: the native-style font, orange lettering and stone-colored frame.
Search Server, Create Server and the waiting room share this presentation.
The online controls remain hidden until the game has loaded and Coco's
waiting area is ready. Select your own compatible original game file first.

Navigate the online menu with the controller's D-pad or left stick. Cross/A
confirms, Circle/B or Start returns, and left/right changes tabs and selection
fields. Holding a direction repeats after a short delay. Confirmation and
Back never repeat; a button held while opening or closing the menu must be
released before it acts in the next screen. Player and server names still use
the keyboard for text entry.

Controller focus now has a visible highlight. Room-list updates preserve the
selected room when possible, disabled choices are skipped, and selection
boundaries do not trigger unnecessary refreshes. Focus also follows text
fields when name validation requires editing.

The existing Start menu keeps Resume, Online Options, Options and Quit. The
original Options settings remain available. Back from Online Options returns
to Start during a game. Quit still leaves the current room and returns to
Coco using the already loaded disc; other players continue, with automatic
host migration when needed.

This release keeps the five-player limit, personal Wumpas, Cloudflare room
discovery and automatic host migration. Multiple independent player windows
on the same PC remain supported.

Validation: all 372 online tests and all 30 desktop tests passed. Coverage
includes the pre-game visibility gate, online menu focus, controller input
mapping, held-button isolation and directional repeat timing. Coco's common
online interface was checked visually. Physical joystick operation was not
validated in this release; automated controller tests do not replace that
check. These checks are not a new complete-level or five-player performance
acceptance.

No disc, ROM, BIOS, personal save, account credential or private database
backup is included. Every player supplies their own compatible original USA
SCUS-94154 game. The app patches a temporary local copy and does not modify the
original file.

This is an unofficial fan project. Crash Bandicoot and associated characters,
names and game assets belong to their respective rights holders. This project
is not affiliated with or endorsed by those rights holders.

[Download for Windows](https://github.com/gabrielcial/crash-double-2-downloads/releases/latest/download/CrashDouble2.exe) · [Website](https://crash-double-2-directory.gabrielcavalcanteoficial.workers.dev/)
