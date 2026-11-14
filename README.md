# Bakuten Shoot Beyblade 2002 - Gekisen! Team Battle!! Seiryuu no Shou - Takao Hen: English Translation

An unofficial English fan translation patch for the Japanese Game Boy Advance game
*Bakuten Shoot Beyblade 2002 - Gekisen! Team Battle!! Seiryuu no Shou - Takao Hen*
(Hudson Soft / Broccoli, 2002). It translates the story, battles, menus, part and launcher
data, and most of the in-game graphics, including the title screen.

## Version

- **Version:** 0.9 beta
- **Release date:** 2026-11-14
- **Format:** BPS patch (`.bps`)

This is a beta. The whole script is translated, but the game has not yet been played from
start to finish on the patched ROM. See [Known issues](#known-issues-and-untranslated-content).

## Required ROM

The patch must be applied to the **unmodified Japanese ROM**. It will not work on another
version (such as *Ouryuu no Shou - Daichi Hen*), on a ROM that has already been patched, or
on a trimmed or headered dump.

| | |
|---|---|
| No-Intro name | `Bakuten Shoot Beyblade 2002 - Gekisen! Team Battle!! Seiryuu no Shou - Takao Hen (Japan)` |
| Game code | `A3WJ` |
| Size | 8,388,608 bytes (8 MB) |
| CRC32 | `8778B36A` |
| MD5 | `a3add916e37dc978a45853703d67d48d` |
| SHA-1 | `30ad2535db0319af509812e67467924164ab640f` |

The BPS format stores the CRC32 of the source ROM, so patchers will refuse a ROM that does
not match.

## Patched ROM (for verification)

| | |
|---|---|
| Size | 16,777,216 bytes (16 MB) |
| CRC32 | `3D33C182` |
| SHA-1 | `d42580f66d9a59a02e33861e36310d22e16954ed` |

The patched ROM is expanded from 8 MB to 16 MB. The extra space holds relocated text and
graphics. This is normal and works on emulators and flash carts.

## How to apply the patch

Keep a backup of your original ROM. The patch creates a new file and does not need to
modify the original.

### Rom Patcher JS (web browser)

1. Open Rom Patcher JS (https://www.marcrobledo.com/RomPatcher.js/).
2. In **ROM file**, select your Japanese `.gba` ROM. The page shows its CRC32; it must be
   `8778B36A`.
3. In **Patch file**, select the `.bps` file from this release.
4. Click **Apply patch** and save the resulting `.gba` file.

### Floating IPS (Flips)

1. Open Flips and choose **Apply Patch**.
2. Select the `.bps` file, then your Japanese `.gba` ROM.
3. Choose a name for the output file and save it.

To check the result, compare the patched ROM's CRC32 or SHA-1 with the values above.

## What is translated

All 6,481 known text entries are translated, inserted and verified against their on-screen
field widths.

- **Story and events:** all story dialogue, cutscenes and tutorials (about 1,300 messages).
- **Battles:** battle messages and commentary (1,872 messages), pre-battle shouts, move
  names, battle commands and special abilities.
- **Menus and interface:** Akebono Town facilities, world map descriptions, team and lineup
  screens, Bey customization, Parts Setup, Launcher Select, Order Select, the name and
  password keyboards (which now open on the Latin alphabet), and the link and GameCube menus.
- **Data:** all Bey part names (1,246 entries) and their descriptions, launchers, team
  names, rival Bey names, random team and Bey names, blader ranks and the staff credits.
- **Names:** bladers keep their original Japanese names in romaji (Takao, Rei, Max, Yuri,
  Seiichi...), and teams keep their original names (Byakko, BBA, PPB, Euro, Borg...), as in
  the Japanese release.
- **Graphics (178 edited graphics resources):**
  - title screen logo and menu
  - world map and Akebono Town labels
  - team banners and the 37 blader name plates
  - battle labels and effects (PLAYER 1/2, CRITICAL, SHOOT!!, GREAT!!...)
  - the results screen (WIN / LOSE / RESULTS)
  - tournament and round titles
  - screen titles and help bars
- **Code changes needed for English text:** the narrow font in message boxes and lists,
  larger line buffers, sprite layout fixes for English labels, and conversion of default Bey
  names in saves created before patching.

## Known issues and untranslated content

- **Beta status:** the game has been played and checked in an emulator during development,
  but no complete playthrough has been done on this version of the patch yet.
- **Link features untested:** link cable battles, part trading, 4-player Simulation Battle
  and GameCube link have not been tested with two devices.
- **Possible small graphic leftovers:** a few edited graphics may still show stray pixels
  from the Japanese originals. The ones under review are the world map labels, the TEAM NAME
  title, NO BIT-BEAST, GAMECUBE LINK, some help bars and the GIMMICK label in the battle HUD.
- **Japanese kana keyboard pages:** the name keyboard still offers its Katakana and Hiragana
  pages, as in the original. It now opens on the Latin page.
- **Internal text left in Japanese:** debug strings, password encryption tables and list
  terminators are not shown during normal play and are intentionally unchanged.
- **Abbreviated names:** the game's fixed-width fields force shortened names in some places
  (for example "Michi", "Gian" and "Kenno" in small fields, and part names of up to 8
  characters when a color suffix follows).
- **Save files:** saves from the Japanese game work with the patch. Bey names that the player
  typed in Japanese stay in Japanese, since they are part of the save data.

## Transparency note

This translation was made with AI assistance. Claude Code (Anthropic) was used to analyze
the ROM, build the extraction and insertion tools, translate the Japanese text, and redraw
the translated graphics. The human author played the patched game in an emulator throughout
development, reviewed the text and graphics on screen, and reported problems that were then
fixed. The text was not reviewed line by line against the Japanese script by a human
translator. If you find a mistranslation or a text that looks wrong in context, please open
an issue with a screenshot.

## Credits

- **manudv:** project lead, testing and review.
- **Claude Code (Anthropic):** ROM analysis, tools, translation and graphics, under the
  direction of manudv.
- **Original game:** Hudson Soft and Broccoli.

## Legal disclaimer

This is an unofficial, non-profit fan project. The patch contains no ROM data and no
copyrighted game files. It only contains the differences needed to modify a ROM you
legally own. No ROMs are provided or linked here, and requests for ROMs will be ignored.

This project is not affiliated with, endorsed by or connected to Takara, Hudson Soft,
Broccoli, Konami or Nintendo. *Beyblade* and all related names and characters are the
property of their respective owners. This patch is distributed free of charge and must not
be sold.

## Changelog

### 0.9 beta (2026-11-14)

- First public release.
- Full script translated: story, battles, tutorials, menus, parts, launchers, teams and
  credits.
- Title screen, maps, banners, name plates, battle effects and results screen translated.
- Name keyboard opens on the Latin alphabet.
- Translation credit line added to the title screen.
