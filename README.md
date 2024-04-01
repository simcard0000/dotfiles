![active development](https://img.shields.io/badge/active%20dev-yes-brightgreen.svg)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/simcard0000/dotfiles.svg)
# dotfiles
☄️ Personal dotfiles for my WSL distribution! Currently under construction. Also contains other information related to workspace setup. Go to:
* [Using a Magic Keyboard with Windows](#using-a-magic-keyboard-with-windows)
* [Files in this Repository](#files-in-this-repository)
* [Notes on Using Chargers/Power Adapters](#notes-on-using-chargerspower-adapters)
* [Other Applications](#other-applications)

### Using a Magic Keyboard with Windows

I have an [Apple Magic Keyboard with Numeric Keypad - US English](https://www.apple.com/ca/shop/product/MQ052LL/A/magic-keyboard-with-numeric-keypad-us-english?afid=p238%7Cstr3DVrrv-dc_mtid_1870765e38482_pcrid_590109978670_pgrid_133662840134_pntwk_g_pchan_online_pexid__&cid=aos-ca-kwgo-pla---slid---product-MQ052LL/A-CA) that I use with a Dell laptop running Windows 11. I remapped some keys on the Apple keyboard using [Microsoft PowerToys](https://learn.microsoft.com/en-us/windows/powertoys/) as such so that they did not interfere with the original keyboard that is part of my laptop:

| Function Key | Previous Key Combo | Does What? |
| ------------ | ------------------ | ----- |
| <kbd>F1</kbd> | N/A | 🌑 switch to dark mode [^1] |
| <kbd>F2</kbd> | N/A | ☀️ switch to light mode |
| <kbd>F3</kbd> | <kbd>⊞ Win</kbd>+<kbd>Tab</kbd> | 🪟 open task view | 
| <kbd>F4</kbd> | <kbd>⊞ Win</kbd>+<kbd>I</kbd> | ⚙️ open Settings |
| <kbd>F5</kbd> | <kbd>⊞ Win</kbd>+<kbd>E</kbd> | 📁 open File Explorer | 
| <kbd>F6</kbd> | <kbd>⊞ Win</kbd>+<kbd>;</kbd> | 😊 open Emoji Panel |
| <kbd>F7</kbd> | <kbd>Previous Track</kbd> | ⏮️ go to previous track |
| <kbd>F8</kbd> | <kbd>Play/Pause Media</kbd> | ⏯️ play/pause media |
| <kbd>F9</kbd> | <kbd>Next Track</kbd> | ⏭️ go to next track |
| <kbd>F10</kbd> | <kbd>Volume Mute</kbd> | 🔇 volume mute |
| <kbd>F11</kbd>| <kbd>Volume Down</kbd> | 🔉 decrease volume |
| <kbd>F12</kbd> | <kbd>Volume Up</kbd> | 🔊 increase volume |
| <kbd>F13</kbd> | <kbd>⊞ Win</kbd>+<kbd>Print Screen</kbd> | 🤳🏽 take a screenshot |
| <kbd>F14</kbd> | <kbd>⊞ Win</kbd>+<kbd>Shift</kbd>+<kbd>C</kbd> | 🎨 open Colour Picker [^2] |
| <kbd>F15</kbd> | <kbd>⊞ Win</kbd>+<kbd>Shift</kbd>+<kbd>M</kbd> | 📏 open Screen Ruler |
| <kbd>F16</kbd> | <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Numpad 1</kbd>

### Files in this Repository

* `.vscode/extensions.json` - list of [VSCode](https://code.visualstudio.com/) extensions that I have currently installed, to be used as [recommendations](https://code.visualstudio.com/docs/editor/extension-marketplace#_workspace-recommended-extensions) in-app.
* `images` - folder of images used in the README for this repo.
* [sims-deep-pink](https://github.com/simcard0000/sims-deep-pink) - 💗 dark theme for Mozilla products with pink highlights - this repository is specified as a submodule in `.gitmodules`.
* `.bashrc` - config for the Bash shell environment.
* `.ssh/config` - config containing saved SSH connection information.

### Notes on Using Chargers/Power Adapters [^3]

1. **Check polarity symbols**: The DC symbol is: ⎓. Look for polarity as a + or - next to the voltage values, or as the below images:

2. **Compare values**: The *input* of the device should be the **same** as the *output* of the adapter - the volts, amperes, and polarity values should all match! There is one other second-best situation though: if the adapter has the *correct voltage* and *polarity* - but the current is *greater* than what the device requires, you should be fine. The following chart shows various combinations from comparing the adapter to the device:

    |Voltage|Amps|Polarity|Ok?|
    |-------|----|--------|---|
    |🟰|🟰|🟰|✅|
    |🟰|⬆️|🟰|✅|
    |🟰|🟰|✖️|❌|
    |⬇️|🟰|🟰|❌|
    |⬆️|🟰|🟰|❌|
    |🟰|⬇️|🟰|❌|

### Other Applications

[^1]: Toggling dark/light mode was done by adapting this tutorial: [Windows Central - How to switch between Windows 10 light and dark modes on schedule automatically](https://www.windowscentral.com/how-switch-between-light-and-dark-colors-schedule-automatically-windows-10), and this "superuser" Stack Exchange question: [Setting a shortcut to trigger task scheduler](https://superuser.com/questions/57694/setting-a-shortcut-to-trigger-task-scheduler).
[^2]: The [Colour Picker](https://learn.microsoft.com/en-us/windows/powertoys/color-picker) and the [Screen Ruler](https://learn.microsoft.com/en-us/windows/powertoys/screen-ruler) are utilities only offered through [Microsoft PowerToys](https://github.com/microsoft/PowerToys).
[^3]: Summarized from: [Complete Guide to Using the Correct Charger or Power Adapter (and What Happens If You Don’t)](https://www.groovypost.com/howto/choose-right-power-adapter-charger-phone-laptop/)