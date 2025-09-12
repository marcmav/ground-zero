# unpacman
### the undo button for pacman

**unpacman** is a tool for Arch Linux and Arch-based distributions that aims to provide a true "undo" for pacman operations.  
It is designed to completely remove packages installed via pacman — including dependencies, extra files, logs, configuration, and metadata — ensuring that everything introduced by a package can be fully undone.

## Features
- Full removal of packages installed via pacman;
- Tracking of changes for clean and reliable uninstalls.  
- Simple, familiar and Arch-focused design.

## How does it work
When you call pacman command to install or update a package, trought hooks system a metadata will be attached to each file that comes from that package ...

## Why This Project
Pacman is a powerful package manager, but sometimes uninstalling a package leaves traces behind.  
**unpacman** was created to explore whether it’s possible to go one step further: to provide a complete rollback mechanism, similar to pressing *Ctrl+Z* for system changes.  


⚠️ Project status: paused — not under active development right now.