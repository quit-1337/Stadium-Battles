<img width="1024" height="640" alt="image" src="https://github.com/user-attachments/assets/9ad6be9d-a923-4dbd-9190-2fbe0e2c881a" />

# Stadium Battles v1.0.2

**Stadium Battles** is a Pokémon Gen 1 / Pokémon Stadium hybrid mod for **Gen1Recomp**.

It keeps the Gen 1 overworld and progression in Gen1Recomp, but routes supported battles into the custom **Pokémon Stadium** runtime for 3D battles. When the battle is over, you return to Gen 1 and continue playing.

Version **v1.0.2** is the current Red / Blue / Yellow release baseline.

## Features

- **Pokémon Red, Blue & Yellow support**
- **Gen 1 battles rendered in Pokémon Stadium**
- **Full Stadium access from the Gen 1 START menu**
- **GB Tower support for Red, Blue & Yellow**
- **Items usable during Stadium battles**
- **Poké Balls and wild Pokémon catching**
- **Gen 1 trainer AI, switching, and item behavior**
- **EXP, level-ups, status, party state, and battle results sync back to Gen 1**
- **Stadium Pokémon storage changes sync back to Gen 1**
- **Full Stadium Pokédex support**
- **Custom arenas based on Gen 1 locations and major battles**
- **Special handling for Safari Zone, Pokémon Tower ghosts, Old Man tutorial, Marowak, Mewtwo, and other unique encounters**

This is **not** a ROM download. Pokémon ROMs are not included.

---

# Downloads

For normal players, download:

`Stadium-Battles-v1.0.2-RED-BLUE-YELLOW.zip`

SHA-256:

```text
6CF23EFC07C68CA5CF5549871B4C7A416AA1312D2D2BCEEDF86B00F84C255D97
```

Source code:

`Stadium-Battles-v1.0.2-SOURCE-COMPLETE.zip`

SHA-256:

```text
438FDA9C0E8778DA5380DD12AA5CB22D14ACF2874B7C2BB4706113CA7E2DDE08
```

The source archive corresponds to the v1.0.2 / r212 release baseline and includes the StadiumRecomp source used for this project, the hybrid integration source, installer/backend scripts, and the presentation-bridge C++ source that was available in the project tree.

---

<img width="1914" height="1003" alt="image" src="https://github.com/user-attachments/assets/a1410b1d-a82d-4722-96b5-9e8035f6091e" />
<img width="833" height="627" alt="image" src="https://github.com/user-attachments/assets/6d67ffb8-b204-4056-bc64-aed18b24caf6" />
<img width="818" height="627" alt="image" src="https://github.com/user-attachments/assets/7a647244-9ba5-4b1a-8073-71ca860f71a5" />
<img width="930" height="627" alt="image" src="https://github.com/user-attachments/assets/fcc6af23-6b54-4989-b5cf-086cc46b6177" />
<img width="1166" height="627" alt="image" src="https://github.com/user-attachments/assets/4bde491f-39f3-4322-b3c3-2f4ae1ebfe83" />



# Requirements

You need:

- **Windows 11**
- A working GPU driver
- A working Gen1Recomp installation
- Your own compatible Pokémon **Red, Blue, or Yellow** ROM for Gen1Recomp
- Your own **Pokémon Stadium USA v1.0 `.z64`** ROM

The Stadium ROM required by this release must have this MD5:

```text
ED1378BC12115F71209A77844965BA50
```

The installer checks this automatically.

No Pokémon ROM is included, downloaded, patched, or modified by Stadium Battles.

The installer also does **not** replace or modify `gen1recomp.exe`.

---

# New User Installation

## 1. Set up Gen1Recomp first

Download and set up Gen1Recomp normally.

If Gen1Recomp is being run for the first time and asks you to select your Pokémon Gen 1 ROM, select your own compatible Pokémon:

- Red
- Blue
- or Yellow

That ROM selection is handled by **Gen1Recomp itself**, not by the Stadium Battles installer.

Make sure Gen1Recomp can launch your game normally before installing Stadium Battles.

## 2. Extract Stadium Battles

Fully extract:

`Stadium-Battles-v1.0.2-RED-BLUE-YELLOW.zip`

Do **not** run the installer from inside the ZIP.

Open the extracted:

`Stadium Battles v1.0.2`

folder.

## 3. Close Gen1Recomp and Stadium

Before installing, close:

- `gen1recomp.exe`
- `PokemonStadiumRecomp.exe`
- any Stadium Battles relay/runtime process

The installer will stop with an error if those processes are still running.

## 4. Run the installer

Double-click:

`RUN-INSTALL.bat`

The installer first verifies the release package and its SHA-256 hashes.

## 5. Select your Gen1Recomp executable

On a new install, you will get a file-selection window asking you to select:

`gen1recomp.exe`

Choose the **same `gen1recomp.exe` that you normally launch to play Gen1Recomp**.

For example, if your Gen1Recomp folder looks like:

```text
gen1recomp-win64\
    gen1recomp.exe
    love.dll
    lua51.dll
    SDL2.dll
```

select:

```text
gen1recomp-win64\gen1recomp.exe
```

The installer uses this selection to find your Gen1Recomp installation folder.

**It does not overwrite or modify `gen1recomp.exe`.**

The installer records its SHA-256 before installation and verifies that the executable is unchanged afterward.

## 6. Select your Pokémon Stadium ROM

On a completely fresh Stadium Battles install, the installer will then display:

```text
[3/5] Select Pokemon Stadium USA v1.0 (.z64).
```

A second file-selection window opens.

Select your own:

```text
Pokemon Stadium (USA) v1.0 .z64
```

The installer verifies that the ROM has this MD5:

```text
ED1378BC12115F71209A77844965BA50
```

If the ROM does not match, installation stops rather than installing against an unsupported Stadium ROM.

You only normally need to select the Stadium ROM **once**.

Its location is remembered in:

```text
%APPDATA%\pokemon-love2d\stadium-battles-runtime\config\stadium-rom.txt
```

On later updates or repair installs, if that file still points to the correct ROM and the ROM still exists, the installer automatically reuses it.

## 7. The install locations are automatic

You are **not** asked to manually choose a Stadium Battles install folder.

The installer determines the correct locations from the `gen1recomp.exe` you selected.

The Stadium runtime is installed under:

```text
%APPDATA%\pokemon-love2d\stadium-battles-runtime
```

For a normal non-portable Gen1Recomp setup, the mod is installed under:

```text
%APPDATA%\pokemon-love2d\mods\STADIUM_BATTLES
```

If your Gen1Recomp installation uses `portable.txt`, the primary mod location is instead:

```text
<your Gen1Recomp folder>\mods\STADIUM_BATTLES
```

The native presentation bridge DLL is installed beside the selected `gen1recomp.exe`.

The installer verifies every deployed release file after installation.

## 8. Launch the game

After the installer reports `PASS`:

1. Launch the same `gen1recomp.exe` you selected during installation.
2. Open the Gen1Recomp **MODS** menu.
3. Enable **Stadium Battles**.
4. Restart Gen1Recomp if it asks you to.
5. Load your Pokémon Red, Blue, or Yellow game normally.

For normal use, launch **Gen1Recomp only**.

You should not need to manually launch `PokemonStadiumRecomp.exe`.

---

# First-Time File Prompts Explained

There are two different programs involved, so first-time setup can involve more than one ROM prompt.

## Gen1Recomp

Gen1Recomp handles your Pokémon Red / Blue / Yellow game.

If it is a fresh Gen1Recomp setup, **Gen1Recomp itself** may ask you where your Gen 1 ROM is located.

Choose your own compatible Red, Blue, or Yellow ROM.

## Stadium Battles installer

The Stadium Battles installer asks for:

### 1. `gen1recomp.exe`

This tells the installer **which Gen1Recomp installation you want to add Stadium Battles to**.

Select the `gen1recomp.exe` you normally launch.

### 2. Pokémon Stadium USA v1.0 `.z64`

This tells Stadium Battles where your Stadium ROM is.

The installer validates it before continuing.

After the first successful install, the Stadium ROM path is saved and normally does not need to be selected again.

The installer does **not** ask you to browse for separate Red, Blue, and Yellow ROMs. Those belong to the Gen1Recomp side of the setup.

---

# Updating From an Older Stadium Battles Version

You do **not** need to uninstall the old version first.

## Recommended update procedure

1. Download the newest Stadium Battles ZIP.
2. Extract it completely to a new folder.
3. Save your game normally.
4. Close Gen1Recomp and Stadium.
5. Run the new `RUN-INSTALL.bat`.
6. Select the same `gen1recomp.exe` you normally use.
7. Let the installer finish.
8. Launch Gen1Recomp normally and make sure Stadium Battles is enabled under **MODS**.

## Will it ask for the Stadium ROM again?

Usually, **no**.

If your previous install has a valid saved Stadium ROM path, the installer prints:

```text
[3/5] Reusing the previously configured Stadium ROM.
```

and continues automatically.

It only asks you to select the Stadium ROM again if the saved path is missing, the ROM was moved/deleted, or the file no longer matches the required ROM.

## What is preserved during an update?

The installer preserves the user cartridge/save information used by the hybrid runtime, including supported Stadium save data and the Transfer Pak configuration.

It also preserves the configured Stadium ROM location.

The new ZIP replaces the actual mod/runtime files with the versions from the new release, including:

- Stadium runtime executable
- mod code
- runtime scripts
- native bridge DLL
- assets
- launcher/input defaults shipped by the release

This prevents old runtime files from being accidentally mixed with a new release.

## Backups

When the installer replaces an existing runtime or mod folder, the previous folder is retained beside it as a:

```text
.before-<transaction>
```

backup.

That gives you a rollback copy of the previous tree if something goes wrong.

---

# How to Use Stadium Battles

Launch:

`gen1recomp.exe`

and play Pokémon Red, Blue, or Yellow normally.

With Stadium Battles enabled, supported Gen 1 battles are handed off to the custom Pokémon Stadium runtime and rendered through the Gen1Recomp window.

When the Stadium battle ends, control returns to the Gen 1 game.

## Full Stadium

Open the Gen 1 START menu and select:

```text
STADIUM
```

This enters the full Stadium runtime.

Use **GO BACK** when you want to return to Gen 1.

## GB Tower

GB Tower is also supported for:

- Pokémon Red
- Pokémon Blue
- Pokémon Yellow

The v1.0.2 baseline was regression-tested across the Red / Blue / Yellow Full Stadium and GB Tower paths.

---

# Troubleshooting

## START → STADIUM does not open

Run:

`GET-STADIUM-ERROR.bat`

The mod records the reason for a failed Stadium launch automatically, and this diagnostic collects the relevant backend and recent game logs.

## Stadium audio works but the picture is black

Leave the failed/black Stadium battle open and run:

`GET-BLACK-SCREEN-DIAGNOSTIC.bat`

The generated report includes information such as:

- running processes
- installed paths
- installed file hashes
- native modules
- GPU / driver information
- Stadium / Gen1 windows
- TCP ports
- backend logs
- recent game logs

The resulting diagnostic is saved in a `Diagnostics` folder beside the release scripts.

When reporting a problem, include the generated diagnostic together with a description of what you were doing when the problem happened.

---

# Release Integrity

The validated v1.0.2 Stadium executable is:

```text
PokemonStadiumRecomp.exe
SHA-256:
EA24C0747A4DA7E4C2B36CEAE8005B8C8342C9196DA9C1AAF9A06C1269F4E05F
```

The validated presentation bridge is:

```text
stadium_shared_present_bridge.dll
SHA-256:
BA4C5D9705EBEBF8D68A295C621F529836EB345326FB2F38539F48B3A0BF1C95
```

The installer verifies the package before installing and verifies the deployed files again afterward.

`gen1recomp.exe` is explicitly excluded from the Stadium Battles payload and is verified to remain unchanged during installation.

---

# Source Code

The corresponding source package is:

`Stadium-Battles-v1.0.2-SOURCE-COMPLETE.zip`

SHA-256:

```text
438FDA9C0E8778DA5380DD12AA5CB22D14ACF2874B7C2BB4706113CA7E2DDE08
```

The generated recomp source is very large when extracted and compresses heavily in the source archive.

The source package includes the available presentation-bridge C++ source as well as the StadiumRecomp/hybrid integration and release integration source used for this project.

---

# Credits

**Stadium Battles mod by KultKlassic**

Built using:

- Gen1Recomp by bryanthaboi  
  https://github.com/bryanthaboi/gen1recomp

- PokemonStadiumRecomp by mstan  
  https://github.com/mstan/PokemonStadiumRecomp

See:

`COPYING-Stadium.txt`

for the PokemonStadiumRecomp licensing information included with the release.

---

# ROMs / Copyright

Stadium Battles does not include Pokémon game ROMs.

Users must provide their own compatible ROMs.

This project is an unofficial fan project and is not affiliated with or endorsed by Nintendo, Game Freak, Creatures, or The Pokémon Company.

Pokémon and related names and properties belong to their respective owners.
