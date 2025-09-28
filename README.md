# ME2_EldenRingMods
A collection of mods made by [techiew](https://github.com/techiew). Refactored to be used with [ModEngine2](https://github.com/soulsmods/ModEngine2/releases). Compatible with Elden Ring 1.16.1.

## Mods:
- [Unlock the framerate](https://www.nexusmods.com/eldenring/mods/216)
- [Remove chromatic aberration](https://www.nexusmods.com/eldenring/mods/179)
- [Remove vignette](https://www.nexusmods.com/eldenring/mods/177)
- [Remove black bars](https://www.nexusmods.com/eldenring/mods/175)
- [Fix the camera](https://www.nexusmods.com/eldenring/mods/118)
- [Pause the game](https://www.nexusmods.com/eldenring/mods/43)
- [Adjust the FoV](https://www.nexusmods.com/eldenring/mods/325) [* not working]
- [Increase animation distance](https://www.nexusmods.com/eldenring/mods/349)
- [Disable rune loss](https://www.nexusmods.com/eldenring/mods/376)
- [Skip the intro](https://www.nexusmods.com/eldenring/mods/421)

## ModEngine2 Example Configurations

- [Seamless Co-op + Item & Enemy Randomizer](_examples/ersc_randomizer.md)

## Compilation
Build under `Release|x64` configuration. A folder in the solution root will be created, labeled `_compiled_mods_yyyy-mm-dd`.

Inside the folder will be all mod .dll files, along with subfolders containing `config.ini` default files (if needed by the mod)

A `build_info.txt` file will be created with Git information pulled from the build machine.

## Credits
- Thanks to **hanslhansl** for [ModEngine2 fix.](https://github.com/techiew/EldenRingMods/issues/15#issuecomment-2233263140)
- Thanks to **uberhalit** for his [EldenRingFpsUnlockAndMore](https://github.com/uberhalit/EldenRingFpsUnlockAndMore) code.
- Thanks to **gurrgur** for his compilation of hex edits in this repo: [er-patcher](https://github.com/gurrgur/er-patcher).
- Thanks to **iArtorias** for his [new pausing technique](https://github.com/iArtorias/elden_pause).
- Thanks to **giniyat202** for his [Linux fix](https://github.com/techiew/EldenRingMods/pull/9).
