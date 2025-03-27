# Command Line Life

## Best Shell

[fish](https://fishshell.com/) -  Finally, a command line shell for the 90s

## Best prompt

[starship](https://starship.rs/) - The cross-shell prompt for astronauts

## Cursors

https://aur.archlinux.org/packages/posy-cursors

## Keyboard configurator

[keyd](https://github.com/rvaiya/keyd)

Configure Left Alt + Space to execute Backspace

```INI
# /etc/keyd/backspace.conf
[ids]
*

[alt]
space = backspace
```

## Shortcuts

Generally working and supported terminal shortcuts.

- `Ctrl + A`: Go to the beninning of a line
- `Ctrl + E`: Go to the end of a line
- `Ctrl + U`: Clear line
- `Ctrl + R`: Search history
- `Ctrl + W`: Remove last word
- `Alt  + S`: Prefix last or current command with sudo

## Commands

Useful commands and utils for working with command line.

- `bat` : a cat clone with wings. https://github.com/sharkdp/bat
- `gdu` : Disk Usage Analyzer https://github.com/dundee/gdu
- `fzf` : FuzZy Finder https://github.com/junegunn/fzf
- `ag`  : The Silver Searcher https://github.com/ggreer/the_silver_searcher
- `eza` : ls replacement written in rust https://github.com/eza-community/eza
- `duf` : Modern disk free / disk usage utility https://github.com/muesli/duf

### Aliases (for Fish Shell)

```shell
# Replace cat with bat
alias --save cat="bat"
# Use fo to search and open with default application
alias --save fo="fzf | xargs -r xdg-open"
# Use eza (exa replacement) to replace ls, ll and la
alias --save ls="eza -hF --icons=always --group-directories-first --git"
alias --save ll="eza -lhF --icons=always --group-directories-first --git"
alias --save la="eza -ahFl --icons=always --group-directories-first --git"
alias --save lsh="eza -hF --icons=always --group-directories-first --git --hyperlink"
# Replace df with duf
alias --save df="duf"
```
