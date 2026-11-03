# Shadows & Seek

A haunted-palace hide-and-hunt game for up to 5 players (1 Shadow vs 4 hunters, bots fill empty seats).
The Shadow hides as the furniture; hunters light the relic candles, then the altar, to banish it.
The Shadow curses shrines to reach the exit, or picks the hunters off from behind.

This repository hosts the **Windows downloads** (see [Releases](../../releases)). Version 0.9.0 is the Palace release.

## Download and run
1. Open the latest release and download the zip. If the zip is split into parts
   (`ShadowsSeek-Palace-0.9.0.zip.part001`, `.part002`, ...), download **all** parts into one folder and join them:
   - Windows Command Prompt, in that folder:
     `copy /b ShadowsSeek-Palace-0.9.0.zip.part001+ShadowsSeek-Palace-0.9.0.zip.part002 ShadowsSeek-Palace-0.9.0.zip`
     (list every part in order, joined with `+`), or run `join-parts.cmd` from the release.
2. Unzip it somewhere you can write to (Desktop or Documents, not Program Files).
3. Start Steam and sign in (lobbies, codes and invites go through Steam), then run `MyProject2.exe`.
4. Windows SmartScreen may warn that the game is not signed: **More info > Run anyway**.
5. Missing `MSVCP140.dll` / `VCRUNTIME140.dll`? Run `Engine\Extras\Redist\en-us\UEPrereqSetup_x64.exe` from the game folder.

The first start compiles shaders ("Preparing the palace", up to a minute or two) and picks a graphics tier for
your PC (change it in Settings > Graphics).

## Controls (all keys can be rebound in Settings > Controls)
| Action | Keyboard / mouse |
|---|---|
| Move / look | W A S D / mouse |
| Jump, skill check | Space |
| Sprint | Shift |
| Use, doors | E |
| Attack | Left mouse |
| Ping | Middle mouse |
| Quick chat (hold) | Z |
| Scoreboard (hold) | Tab |
| Push to talk | T |
| Reload / hunter ability / chalk mark | R / Q / X |
| Shadow abilities, Hunter's Guise, Stolen Voice, Jumpscare | 1-5, 6, 7, G |
| Menu / bug report | Esc or M / F8 |

**Controller (Xbox layout):** left stick moves, right stick looks; in menus the D-pad moves and A selects, B goes
back. The full controller layout is in Settings > Controls.
**Controller vs bots (offline):** double-click `Play with controller (offline).cmd` next to the exe; it starts without Steam, so the pad works at once.
Controller not responding online? In Steam: Library > Spacewar > Properties > Controller > Disable Steam Input, then restart the game.

## PC requirements
- Windows 10 or 11 (64-bit), DirectX 12, 16 GB RAM, about 10 GB free disk.
- Minimum: GTX 1060 6 GB / RX 580 class GPU, 4-core CPU (Low tier).
- Recommended: RTX 3060 / RX 6600 class or better (High tier, 60+ fps).

## Known issues
- Steam shows the game as "Spacewar" (Steam's test app) until the store page exists.
- Saves and settings stay on your PC (`%LOCALAPPDATA%\MyProject2\Saved`). If the game crashes, please send the newest
  folder in `%LOCALAPPDATA%\MyProject2\Saved\Crashes`, or press F8 in game to save a bug report.
- Ranked is a beta and the store is a preview (nothing costs money).
- The Opera House and the Mall are not in this release (Palace only).

## Coming in 0.9.1
- Native Steam Input controller support (no Steam setting needed).

## Credits
Third-party credits and licences ship with the game in `THIRD-PARTY-NOTICES.txt` and the `OFL-*.txt` font licences
(Gothic props by E.Bolday, CC BY 4.0; 100STYLE motion data, CC BY 4.0; Cinzel and EB Garamond, SIL OFL 1.1; CC0 assets
from KayKit, Kenney, OpenGameArt, Poly Haven and ambientCG). Made with Unreal(R) Engine.
