# Eleftheria Anastasia's Recommended MacOS Setup and Applications

## Terminal

### Terminal emulator

The built-in terminal emulator is not very good.
I highly recommend using [iTerm2](https://iterm2.com/downloads.html).

Others might recommend using different emulators.
I'm sure that they're all decent; however, I have my own reasons for not using them:

- [ghostty](https://ghostty.org/): Ghostty works great and is super fast. I personally don't use it because (when I tried it) it didn't cooperate very well with sshing into the Linux computing clusters I use for research (see [this article](https://ghostty.org/docs/help/terminfo) for more info).
- [Alacritty](https://alacritty.org/): I personally just found iTerm2 to be nicer and simpler to use.
- [Kitty](https://sw.kovidgoyal.net/kitty/): I don't think I've ever used this one because I like iTerm2 enough.

### Shell

Since macOS Catalina (10.15), the default shell on macOS is zsh.
You can change your shell using the [Terminal app](https://support.apple.com/guide/terminal/change-the-default-shell-trml113/mac) or using the [`chsh` command](https://www.man7.org/linux/man-pages/man1/chsh.1.html) as you would on any Unix system.

Personally, I would recommend against changing your default shell because macOS and programs designed for macOS are now being made to work with zsh by default.
However, I know that zsh may not have all the features you like (especially if you're used to using fish).
I recommend using [Oh My Zsh](https://ohmyz.sh/) with zsh to get a lot of those missing features.

### Shell programs

Note that macOS ships with its own versions of shell programs.
Therefore, commands that you're used to on Linux likely do not work the exact same way on macOS as they do on Linux.
Make use of macOS manpages for more.

## Python

MacOS ships with a default Python installation, located at `usr/bin`.
**DO NOT USE THIS PYTHON EVER.**
This Python is the system Python and is used by the operating system and/or default macOS applications.

To use Python for you own purposes, you need to download your own Python binary.
See [below](#Python-versions) for my recommendations for doing so.
I highly recommend AGAINST using Homebrew or another macOS package manager to install and manage Python versions.

## Package management

### MacOS packages

[Homebrew](https://brew.sh/)

[MacPorts](https://www.macports.org/)

### Python versions

[pyenv](https://github.com/pyenv/pyenv)

### Julia versions

[juliaup](https://github.com/JuliaLang/juliaup)

## Finder

### OpenInTerminal

[OpenInTerminal](https://github.com/Ji4n1ng/OpenInTerminal)

### Syntax Highlight

[Syntax Highlight](https://sbarex.github.io/SourceCodeSyntaxHighlight/)

## Window management

[Rectangle](https://rectangleapp.com/)

## Keyboard customization

I use [Karabiner Elements](https://karabiner-elements.pqrs.org/) to add complex keybindings that work system-wide.
I primarily use this to make it easier to type `_`s.
Some of my Karabiner Elements modifications are [here](karabiner-elements-modifications.md).

## System management

[Stats](https://mac-stats.com/)

### Storage management

[DaisyDisk](https://daisydiskapp.com/)

### Audio management

[SoundSource](https://rogueamoeba.com/soundsource/)

## LaTeX

[MacTeX](https://www.tug.org/mactex/)

### LaTeX editor

[TeXstudio](https://www.texstudio.org/)

[TeXShop](https://pages.uoregon.edu/koch/texshop/)

[Texifier](https://www.texifier.com/)

[Visual Studio Code](https://code.visualstudio.com/) + [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) + [LTeX+](https://marketplace.visualstudio.com/items?itemName=ltex-plus.vscode-ltex-plus)

## Multiple displays

[DisplayLink Manager](https://www.synaptics.com/products/displaylink-graphics/downloads/macos)

## Git

Note, macOS by default almost always creates a [`.DS_Store` file in folders](https://en.wikipedia.org/wiki/.DS_Store).
As a result, you always need a `.gitignore` file that always includes `.DS_Store` in git repositories.

### GitHub

[GitHub CLI](https://cli.github.com/)

## Linux on Apple Silicon

**PROCEED AT YOUR OWN RISK!**

If you decide you must install a true Linux distribution on your Mac, [Asahi Linux](https://asahilinux.org/) is the way to go.
