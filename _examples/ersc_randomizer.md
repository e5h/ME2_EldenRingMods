# Seamless Co-op + Item & Enemy Randomizer

## Config File

[Note: AdjustTheFov is not included in this configuration - mod appears incompatible]

`config_eldenring.toml`

```
# Global mod engine configuration
[modengine]
# If set to true the debug console will appear while the game is running
debug = false

external_dlls = [
	"mod\\SkipTheIntro.dll",
	"mod\\UltrawideFix.dll",
	"mod\\RemoveVignette.dll",
	"mod\\RemoveChromaticAberration.dll",
	"mod\\IncreaseAnimationDistance.dll",
	"mod\\UnlockTheFps.dll",
	"mod\\SeamlessCoop\\ersc.dll",
]

# Mod loader configuration
[extension.mod_loader]
enabled = true

# Not currently supported for Elden Ring
loose_params = false

# Additional mod directories
mods = [
	{ enabled = true, name = "SkipTheIntro", path = "mod\\SkipTheIntro" },
	{ enabled = true, name = "default", path = "randomizer" },
	{ enabled = true, name = "UnlockTheFps", path = "mod\\UnlockTheFps" },
	{ enabled = true, name = "SeamlessCoop", path = "mod\\SeamlessCoop" },
]

# When enabled, scylla hide will be injected into the game. This allows for antidebug measures in the game to be bypassed so that you can attach
# debuggers such as Cheat Engine, x64dbg, windbg, etc to the game without as much trouble. If you're not reverse engineering the game, this option
# is probably not for you.
[extension.scylla_hide]
enabled = false
```

## Folder Structure

```
.
└── ModEngine2_Launch_Folder/
    ├── mod/
    │   ├── AdjustTheFov/
    │   │   └── config.ini
    │   ├── SeamlessCoop/
    │   │   ├── crashpad/...
    │   │   ├── locale/...
    │   │   ├── ersc.dll
    │   │   └── ersc_settings.ini
    │   ├── SkipTheIntro/
    │   │   └── config.ini
    │   └── UnlockTheFps/
    │       └── config.ini
    ├── modengine2/
    │   ├── assets/...
    │   ├── bin/...
    │   ├── crashpad/...
    │   ├── include/...
    │   ├── lib/...
    │   ├── logs/...
    │   ├── share/...
    │   └── tools/...
    ├── randomizer/
    │   ├── diste/...
    │   ├── dll/...
    │   ├── event/...
    │   ├── map/...
    │   ├── msg/...
    │   ├── script/...
    │   ├── sfx/...
    │   ├── spoiler_logs/...
    │   ├── config_eldenringrandomizer.toml
    │   ├── EldenRingRandomizer.exe
    │   ├── libzstd.dll
    │   ├── oo2core_6_win64.dll
    │   ├── README.txt
    │   └── regulation.bin
    ├── config_eldenring.toml
    ├── launchmod_eldenring.bat
    ├── modengine2_launcher.exe
    └── README.txt
```

## Other Instructions

- Run the `EldenRingRandomizer.exe` application to generate files
- Zip the entire randomizer folder to distribute to friends
- Use `launchmod_eldenring.bat` to start the game
- ModEngine2 seems to cache something. After loading these mods, if the game crashes, just launch again. It should resolve.