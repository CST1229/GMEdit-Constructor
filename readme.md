# GMEdit-Constructor
As the title suggests, Constructor is a plugin for YellowAfterlife's [GMEdit](<https://github.com/YellowAfterlife/GMEdit>), which allows you to compile from the editor just as you can in the GameMaker IDE.

Currently, Constructor about matches the capabilities of [builder](<https://github.com/YAL-GMEdit/builder>), which is another plugin serving the same role, but as GM now uses Igor as a commandline tool to automate things, it means that interacting with the compiler is a lot easier and a lot less error-prone (especially as GM changes, which invoking the AssetCompiler directly cannot cope with.)

Constructor can currently compile for the current build target (your OS), and can switch between build configs.

## Features
 - [x] **Run compile, run and clean jobs** (technically can be in parallel!)
   - [x] Stop jobs by closing their tab
 - [x] **View compile output** (duh)
 - [x] **Compile and runner error parsing** (view them nice and neat rather than scrolling the log!)
 - [x] **Runtime selection & project-specific properties**
   - [x] Project build configuration select (`#macro SOMETHING:Config ...` support)
 - [x] **Control Panel** (*see screenshot below*)
   - [x] Centralised error display for build and configuration problems

![image](https://github.com/thennothinghappened/GMEdit-Constructor/assets/35243139/6cde8fc7-ed20-4680-88a3-9207c5b0b938)

## Installation
Installation is the same here as any other GMEdit plugin - clone it into your `plugins` folder (see below), or download the `.zip` from *Releases*, and extract the contained folder into `plugins`.

### Windows
```sh
git clone https://github.com/thennothinghappened/GMEdit-Constructor %appdata%\AceGM\GMEdit\plugins\GMEdit-Constructor
```

### MacOS
```sh
git clone https://github.com/thennothinghappened/GMEdit-Constructor ~/Library/Application Support/AceGM/GMEdit/plugins/GMEdit-Constructor
```

See [GMEdit#Installing plugins](https://github.com/YellowAfterlife/GMEdit/wiki/Using-plugins#installing-plugins)
for more details!

## Shortcuts

| Shortcut          | Key                |
| ----------------- | ------------------ |
| **Control Panel** | <kbd>Ctrl+\`</kbd> |
| **Compile**       | <kbd>Ctrl+F5</kbd> |
| **Clean**         | <kbd>Ctrl+F7</kbd> |
| **Run**           | <kbd>F5</kbd>      |

Maybe later these can be customisable :)

## Planned features include:
- **Support for other targets**:
  - HTML5
  - Android
  - Remote compilation for other platforms using `devices.json` (compile on another machine via `ssh` as you can in the IDE)
- YYC support
- Option for docked console as opposed to full-window

## Issues
If you have any issues with Constructor, feel free to either ask on Discord (below), or make a post on the [GitHub Issues](<https://github.com/thennothinghappened/GMEdit-Constructor/issues>) page. I'll try to get back to you when I can, but no guarantees.

## Feature requests
If there's anything else you'd like out of Constructor that isn't mentioned here, the same applies as above with issues - make a feature request by opening an issue on GitHub!

I hope Constructor is a useful tool - though please note that I can only test on the machines I have available to me, so there's gonna be edge cases.

Finally, I also have a thread for this project on the [GameMaker Kitchen Discord server](https://discord.com/channels/724320164371497020/1208360272570490930), for quick feedback!

Thanks, and have fun :)
