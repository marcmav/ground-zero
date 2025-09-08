# unpacman
### the undo button for pacman

**unpacman** is a tool for Arch Linux and Arch-based distributions that completely removes packages installed via pacman, includes all dependencies, extra files, logs, configuration, metadata and essentially everything that entered on your machine with the package installed via pacman ensuring that you undo the pacman command.

## Features
- Full removal of packages installed via pacman;
- Tracks all changes for a clean uninstall;
- Simple, familiar and Arch-focused.

## How does it work
When you call pacman command to install or update a package, trought hooks system a label (unpacman-label) is attached to all files that comes from that same package ...