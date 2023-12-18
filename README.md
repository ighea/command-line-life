# Command Line Life

## Best Shell

fish

## Shortcuts

Generally working and supported terminal shortcuts.

- `Ctrl + A`: Go to the beninning of a line
- `Ctrl + E`: Go to the end of a line
- `Ctrl + U`: Clear line
- `Ctrl + R`: Search history
- `Ctrl + W`: Remove last word
- `Alt + s`: Last command, but with sudo

## Commands

Useful commands and utils for working with command line.

- `bat` : a cat clone with wings.
- `gdu` : Disk Usage Analyzer
- `fzf` : FuzZy Finder
- `ag`  : The Silver Searcher
- `eza` : ls replacement written in rust

### Aliases (for Fish Shell)

```shell
# Replace cat with bat
alias --save cat="bat"
# Use fo to search and open with default application
alias --save fo="fzf | xargs -r xdg-open"
# Use eza (exa replacement) to replace ls, ll and la
alias --save ls="eza -hF --icons=always --group-directories-first"
alias --save ll="eza -lhF --icons=always --group-directories-first"
alias --save la="eza -ahFl --icons=always --group-directories-first"
```
