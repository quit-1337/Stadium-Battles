<img width="1024" height="640" alt="Stadium Battles" src="https://github.com/user-attachments/assets/9ad6be9d-a923-4dbd-9190-2fbe0e2c881a" />

# Stadium Battles v1.0.19

**Stadium Battles** is a Pokémon Gen 1 / Pokémon Stadium hybrid mod for **Gen1Recomp**.

Stadium Battles seamlessly connects Gen1Recomp with Pokémon Stadium, letting you battle with your Gen 1 team and play the full Stadium experience with instant connectivity between both games.

Play the Gen 1 overworld, story, and progression in Gen1Recomp, with battles and encounters handled in Pokémon Stadium. When a battle ends, you return directly to Gen 1. You can also open the full Stadium game from the START menu and use your Gen 1 Pokémon in Stadium.

Version **v1.0.19** supports Pokémon Red, Blue, and Yellow.

## Features

- **Pokémon Red, Blue & Yellow support**
- **Gen 1 battles rendered in Pokémon Stadium**
- **Play the full Pokémon Stadium game with your Gen 1 Pokémon, directly from the START menu**
- **GB Tower support for Red, Blue & Yellow**
- **Items usable during Stadium battles**
- **Poké Balls and wild Pokémon catching**
- **Gen 1 trainer AI, switching, and item behavior**
- **EXP, level-ups, status, party state, and battle results sync back to Gen 1**
- **Stadium changes sync back to Gen 1**
- **Optional Kids’ Club minigame Stat Exp and DV training for your Gen 1 party**
- **Saved view settings, opponent HP display options, and Stadium control bindings**
- **Custom arenas based on Gen 1 locations and major battles**
- **Special handling for Safari Zone, Pokémon Tower ghosts, Old Man tutorial, and other unique encounters**

This is **not** a ROM download. Pokémon ROMs are not included.

---

## Downloads

To play the mod, download:

`STADIUM_BATTLES-1.0.19.zip`

For development, download the source code:

`STADIUM_BATTLES-1.0.19-SOURCE.zip`

---

## Install

**Windows 64-bit only.**

You need:

- A working Gen1Recomp installation with Pokémon Red, Blue, or Yellow already set up
- Your own legally obtained Pokémon Stadium USA v1.0 ROM (`.z64`, `.n64`, or `.v64`)

Then:

1. Download `STADIUM_BATTLES-1.0.19.zip`. **Do not extract it.**
2. Open **MODS** in Gen1Recomp and import the ZIP.
3. Supply your Pokémon Stadium USA v1.0 ROM when the launcher asks for the mod's required ROM.
4. Start Pokémon Red, Blue, or Yellow.
5. Wait while the first launch quickly prepares the Stadium runtime automatically and play.

## Pokémon Stadium ROM

Supported formats:

- `.z64`
- `.n64`
- `.v64`

Canonical Pokémon Stadium USA v1.0 `.z64` MD5:

`ED1378BC12115F71209A77844965BA50`

No commercial Pokémon ROMs are included.

## Updating

The Gen1Recomp launcher checks `quit-1337/Stadium-Battles` on GitHub for new releases. Choose **Update** in **MODS** when a newer release is available.

Close Pokémon Stadium before updating. Fully close and reopen Gen1Recomp after the update so the bundled runtime and presentation DLL can be updated safely.

**Do not uninstall the old version first.**

Your existing ROMs, saves, and personal settings are preserved during an update.

## Using Stadium Battles

Launch Gen1Recomp normally and play Pokémon Red, Blue, or Yellow.

Battles are handed off to Pokémon Stadium automatically. When the battle ends, you return directly to Gen 1.

## Full Stadium

Open the Gen 1 START menu and select:

`STADIUM`

Use your Gen 1 Pokémon in the full Stadium game, including its regular battle modes, Pokémon Lab, GB Tower, and Kids’ Club.

Use **GO BACK** when you want to return to Gen 1. Supported party, storage, and save changes are synced back to your adventure.

## Stadium Options

Open **OPTIONS → STADIUM OPTIONS** in Gen1Recomp to customize the mod.

| Setting | What it does |
| --- | --- |
| **MINIGAME STAT TRAINING** | Turns party training rewards from Kids’ Club wins on or off. Enabled by default. |
| **OPPONENT HP** | Chooses the original Red/Blue/Yellow HP display or Stadium’s native HP display. |
| **UNCROPPED** | Expands the Stadium view to fit your window. Turn it off for the original 4:3 view. |
| **STADIUM CONTROLS** | Opens keyboard and controller button bindings for Stadium. |

Your choices are saved. Use Up/Down to select a setting and Left/Right to change it. Press A to open control bindings, SELECT for more help, and B to go back.

## Kids’ Club Training

With **MINIGAME STAT TRAINING** enabled, eligible Player 1 wins in Kids’ Club train the Gen 1 Pokémon in your party at the time of the win.

| Minigame | Stat trained |
| --- | --- |
| Magikarp’s Splash; Ekans’ Hoop Hurl | Attack |
| Rock Harden; Dig! Dig! Dig! | Defense |
| Run, Rattata, Run; Thundering Dynamo | Speed |
| Clefairy Says; Snore War | Special |
| Sushi-Go-Round | HP |

Higher difficulties give more stat experience. Hard and Hyper wins also improve the corresponding non-HP DV by 1, up to 15. DVs are Gen 1’s innate stat values. Sushi-Go-Round gives extra HP stat experience instead of a direct HP DV reward.

Minigame training raises stat experience up to 50,000 per stat.

Wins are recorded while you play Stadium. **Choose GO BACK to apply the rewards to Gen 1.** Saving afterward keeps the earned gains. Turning training off keeps saved gains but cancels rewards that have not yet been applied.

Player 2, 3, and 4 wins do not grant training rewards to your Gen 1 party. Multiplayer minigames remain playable.

## FAQ

### Can I use my existing Gen 1 save?

Yes. Continue your configured Red, Blue, or Yellow game in Gen1Recomp. Installing or updating the mod preserves your existing ROMs, saves, and personal settings.

### Do I launch Pokémon Stadium separately?

Launch Gen1Recomp normally. Stadium Battles starts the Stadium runtime when needed and displays it inside the Gen1Recomp window.

### Is this only for battles during the Gen 1 adventure?

You can also play the full Pokémon Stadium game with your Gen 1 Pokémon. Open **STADIUM** from the Gen 1 START menu and choose **GO BACK** to return.

### Can I catch wild Pokémon and use items?

Yes. Supported adventure battles allow items and Poké Balls, with catches and battle results carried back to Gen 1. Trainer Pokémon cannot be caught. Running is available in wild battles and blocked in trainer battles.

### Do minigame rewards increase my stats as soon as I win?

The win is recorded in Stadium. The training gains are applied when you return to Gen 1 with **GO BACK**. You do not need to level up first, and saving afterward does not erase the rewards. The minigame rewards can be turned off in the Stadium Options.

### Can I keep the original Stadium screen shape?

Yes. Turn **UNCROPPED** off in **STADIUM OPTIONS** for the original 4:3 view.

### Can I use other Gen1Recomp mods at the same time?

Compatibility depends on what the other mods change. Mods that replace battle behavior, menus, input, or rendering may conflict. If you encounter a problem, try Stadium Battles by itself to help identify the cause.

### Should I extract the player ZIP or install the source ZIP?

Import `STADIUM_BATTLES-1.0.19.zip` directly through **MODS** without extracting it. The `SOURCE` ZIP is for development.

## Uninstalling

Close Gen1Recomp and Pokémon Stadium, then run `RUN-UNINSTALL.bat` from the installed mod folder. It removes the installed software while keeping saves, ROMs, and personal settings.

Removing the mod through the launcher alone leaves the separately installed Stadium runtime behind. Use the bundled uninstaller first for a complete uninstall.

## Reporting Problems

Report problems through [GitHub Issues](https://github.com/quit-1337/Stadium-Battles/issues). Include:

- Your Stadium Battles and Gen1Recomp versions
- Whether you are playing Red, Blue, or Yellow
- The steps that trigger the problem and what happened
- Whether it happens in an adventure battle or Full Stadium
- Any error message, and a screenshot or short video if useful
- Whether other mods are enabled

## Source Code

The source download is `STADIUM_BATTLES-1.0.19-SOURCE.zip`. For build instructions, see `PokemonStadiumRecomp/BUILDING.md` inside the source archive.

## Credits

**Stadium Battles mod by KultKlassic**

Stadium Battles would not be possible without:

- **[Gen1Recomp](https://github.com/bryanthaboi/gen1recomp)** by [bryanthaboi](https://github.com/bryanthaboi) — the Gen 1 recompilation/runtime that Stadium Battles integrates with
- **[PokemonStadiumRecomp](https://github.com/mstan/PokemonStadiumRecomp)** by [mstan](https://github.com/mstan) — the Pokémon Stadium recompilation that powers the 3D battle side of the mod

Huge thanks to the developers and contributors behind both projects for making Stadium Battles possible.

SPECIAL THANKS TO TESTERS: sickflip, Quinn, parafwen, Kai

See `COPYING-Stadium.txt` for the PokemonStadiumRecomp licensing information included with the release.

## ROMs / Copyright

Stadium Battles does not include Pokémon game ROMs. Users must provide their own compatible ROMs.

Stadium Battles is an unofficial fan-made project and is not affiliated with or endorsed by Nintendo, Game Freak, Creatures, or The Pokémon Company.

Pokémon and related names and properties belong to their respective owners.

<img width="1914" height="1003" alt="Stadium Battles gameplay" src="https://github.com/user-attachments/assets/a1410b1d-a82d-4722-96b5-9e8035f6091e" />
<img width="833" height="627" alt="Stadium Battles gameplay" src="https://github.com/user-attachments/assets/6d67ffb8-b204-4056-bc64-aed18b24caf6" />
<img width="818" height="627" alt="Stadium Battles gameplay" src="https://github.com/user-attachments/assets/7a647244-9ba5-4b1a-8073-71ca860f71a5" />
<img width="930" height="627" alt="Stadium Battles gameplay" src="https://github.com/user-attachments/assets/fcc6af23-6b54-4989-b5cf-086cc46b6177" />
<img width="1166" height="627" alt="Stadium Battles gameplay" src="https://github.com/user-attachments/assets/4bde491f-39f3-4322-b3c3-2f4ae1ebfe83" />


