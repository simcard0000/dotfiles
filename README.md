![active development](https://img.shields.io/badge/active%20dev-on%20hold-yellow.svg)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/simcard0000/dotfiles.svg)
# dotfiles
☄️ Personal dotfiles for my WSL distribution! Currently under construction. Also contains other information related to workspace setup.

### Using a Magic Keyboard with Windows

I have an [Apple Magic Keyboard with Numeric Keypad - US English](https://www.apple.com/ca/shop/product/MQ052LL/A/magic-keyboard-with-numeric-keypad-us-english?afid=p238%7Cstr3DVrrv-dc_mtid_1870765e38482_pcrid_590109978670_pgrid_133662840134_pntwk_g_pchan_online_pexid__&cid=aos-ca-kwgo-pla---slid---product-MQ052LL/A-CA) that I use with a Dell laptop running Windows 11. I remapped some keys on the Apple keyboard using [Microsoft PowerToys](https://learn.microsoft.com/en-us/windows/powertoys/) as such so that they did not interfere with the original keyboard that is part of my laptop:
  * <kbd>F1</kbd> **Switch to Dark Mode** and <kbd>F2</kbd> **Switch to Light Mode**
    
    The following instructions are adapted from this tutorial: [Windows Central - How to switch between Windows 10 light and dark modes on schedule automatically](https://www.windowscentral.com/how-switch-between-light-and-dark-colors-schedule-automatically-windows-10), and this "superuser" Stack Exchange question: [Setting a shortcut to trigger task scheduler](https://superuser.com/questions/57694/setting-a-shortcut-to-trigger-task-scheduler).
    
      1. Open up the Task Scheduler application, expand the "Task Scheduler Library" folder, and create a new folder within. This folder will help differentiate between custom tasks and pre-defined system tasks.
      2. In the newly created folder, create a new task (select the "Create Task" option).

  * <kbd>F3</kbd>: <kbd>⊞ Win</kbd>+<kbd>Tab</kbd> **Open Task view**
  * <kbd>F4</kbd>: <kbd>⊞ Win</kbd>+<kbd>I</kbd> **Open Settings**
  * <kbd>F5</kbd>: <kbd>⊞ Win</kbd>+<kbd>E</kbd> **Open File Explorer**
  * <kbd>F6</kbd>: <kbd>⊞ Win</kbd>+<kbd>;</kbd> **Open emoji panel**
  * <kbd>F7</kbd>: <kbd>Previous Track</kbd>
  * <kbd>F8</kbd>: <kbd>Play/Pause Media</kbd>
  * <kbd>F9</kbd>: <kbd>Next Track</kbd>
  * <kbd>F10</kbd>: <kbd>Volume Mute</kbd>
  * <kbd>F11</kbd>: <kbd>Volume Down</kbd>
  * <kbd>F12</kbd>: <kbd>Volume Up</kbd>
  * <kbd>F13</kbd>: <kbd>⊞ Win</kbd>+<kbd>Print Screen</kbd>
  * <kbd>F14</kbd>: <kbd>⊞ Win</kbd>+<kbd>Shift</kbd>+<kbd>C</kbd> **Open Colour Picker**
  * <kbd>F15</kbd>: <kbd>⊞ Win</kbd>+<kbd>Shift</kbd>+<kbd>M</kbd> **Open Screen Ruler**
  * <kbd>F16</kbd>: <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Numpad 1</kbd>
