![active development](https://img.shields.io/badge/active%20dev-yes-brightgreen.svg)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/simcard0000/dotfiles.svg)
# dotfiles
☄️ Personal dotfiles for my WSL distribution! Currently under construction. Also contains other information related to workspace setup. Go to:
* [Useful Links](#useful-links)
* [Using a Magic Keyboard with Windows](#using-a-magic-keyboard-with-windows)
* [Files in this Repository](#files-in-this-repository)
* [Notes on Using Chargers/Power Adapters](#notes-on-using-chargerspower-adapters)
* [Other Applications](#other-applications)

### Useful Links
* [Setting Up a UWaterloo Email with Mozilla Thunderbird](https://cs.uwaterloo.ca/twiki/view/CrySP/UWaterlooEmailThunderbird)

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
* `.ssh/config` - config containing saved SSH connection information - needs [comments stripped before use](https://github.com/getify/JSON.minify/tree/python).

### Notes on Using Chargers/Power Adapters [^3]

1. **Check polarity symbols**: The DC symbol is: ⎓. Look for polarity as a + or - next to the voltage values, or as the below image:
   
   ![polarity symbols](https://github.com/simcard0000/dotfiles/blob/main/images/AC_adaptor_polarity.png)[^4]

3. **Compare values**: The *input* of the device should be the **same** as the *output* of the adapter - the volts, amperes, and polarity values should all match! There is one other second-best situation though: if the adapter has the *correct voltage* and *polarity* - but the current is *greater* than what the device requires, you should be fine. The following chart shows various combinations from comparing the adapter to the device:

    |Voltage|Amps|Polarity|Ok?|
    |-------|----|--------|---|
    |🟰|🟰|🟰|✅|
    |🟰|⬆️|🟰|✅|
    |🟰|🟰|✖️|❌|
    |⬇️|🟰|🟰|❌|
    |⬆️|🟰|🟰|❌|
    |🟰|⬇️|🟰|❌|

### Other Applications
This is a list of things I have installed on my computer; however, it is not exhaustive. Most of these apps I use often, but there are some that I no longer open - so this list needs to eventually get pruned.

* Office 365 Suite (Word, PowerPoint, OneNote, etc.) → [get from UWaterloo](https://uwaterloo.ca/microsoft-365/)
* [Adobe Acrobat DC/Reader (free version)](https://www.adobe.com/ca/acrobat/pdf-reader.html)
* [Anaconda Navigator](https://www.anaconda.com/anaconda-navigator)
    * [Jupyter Notebook](https://jupyter.org/)
    * [Spyder IDE](https://www.spyder-ide.org/)
* [Cygwin](https://www.cygwin.com/) / [MYSYS2](https://www.msys2.org/) / [MinGW](https://www.mingw-w64.org/) - some useful installation tutorials include: [Cygwin64 & MinGW-w64 (for Windows) - How To Install and Get Started](https://www3.ntu.edu.sg/home/ehchua/programming/howto/Cygwin_HowTo.html) and [My Ultimate Cygwin Setup](https://guysherman.com/2013/11/02/my-ultimate-cygwin-setup/)
* [Docker Desktop](https://www.docker.com/products/docker-desktop/)
* [Google Cloud SDK](https://cloud.google.com/sdk)
* [Eclipse IDE](https://eclipseide.org/)
* [Java Development Kit - JDK](https://www.oracle.com/ca-en/java/technologies/downloads/)
* [ANTLR](https://www.antlr.org/)
* [Mozilla FireFox](https://www.mozilla.org/en-CA/firefox/)
* [Mozilla Thunderbird](https://www.thunderbird.net/en-CA/)
* [Git](https://git-scm.com/)
* [GitHub Desktop](https://desktop.github.com/)
* [Gluon SceneBuilder](https://gluonhq.com/products/scene-builder/)
* [Inform 7](https://ganelson.github.io/inform-website/)
* [Kong - Insomnia](https://insomnia.rest/)
* [Microsoft Whiteboard](https://www.microsoft.com/en-ca/microsoft-365/microsoft-whiteboard/digital-whiteboard-app)
* [Node.js](https://nodejs.org/en)
* [Notion](https://www.notion.so/)
* [AnyType](https://anytype.io/)
* [PICO-8](https://www.lexaloffle.com/pico-8.php)
* [Bitwarden](https://bitwarden.com/)
* [Postgresql](https://www.postgresql.org/)
* [PuTTY](https://www.putty.org/)
* [Python](https://www.python.org/)
* [Spotify](https://open.spotify.com/)
* [Twine](https://twinery.org/)
* [Visual Studio](https://visualstudio.microsoft.com/)
* [Go Language](https://go.dev/)
* [Dart](https://dart.dev/)
* [Flutter](https://flutter.dev/)
* [Figma](https://www.figma.com/)
* [FontForge](https://fontforge.org/en-US/)
* [Inkscape](https://inkscape.org/)
* [draw.io](https://app.diagrams.net/)
* [Zotero](https://www.zotero.org/)
* [Audacity](https://www.audacityteam.org/)
* [CMake](https://cmake.org/)
* [iTunes](https://support.apple.com/en-ca/HT210384)
  
[^1]: Toggling dark/light mode was done by adapting this tutorial: [Windows Central - How to switch between Windows 10 light and dark modes on schedule automatically](https://www.windowscentral.com/how-switch-between-light-and-dark-colors-schedule-automatically-windows-10), and this "superuser" Stack Exchange question: [Setting a shortcut to trigger task scheduler](https://superuser.com/questions/57694/setting-a-shortcut-to-trigger-task-scheduler).
[^2]: The [Colour Picker](https://learn.microsoft.com/en-us/windows/powertoys/color-picker) and the [Screen Ruler](https://learn.microsoft.com/en-us/windows/powertoys/screen-ruler) are utilities only offered through [Microsoft PowerToys](https://github.com/microsoft/PowerToys).
[^3]: Summarized from: [Complete Guide to Using the Correct Charger or Power Adapter (and What Happens If You Don’t)](https://www.groovypost.com/howto/choose-right-power-adapter-charger-phone-laptop/).
[^4]: [AC_adaptor_polarity.png](https://en.wikipedia.org/wiki/Polarity_symbols#/media/File:AC_adaptor_polarity.png) and [license](https://creativecommons.org/licenses/by-sa/3.0/).
