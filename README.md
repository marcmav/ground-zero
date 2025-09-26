# unpacman

### The undo button for pacman.

**unpacman** is a tool for Arch Linux and Arch-based distributions that aims to provide a true "undo" for pacman operations.  
It is designed to completely remove packages installed via pacman — including dependencies, extra files, logs, configuration, and metadata — ensuring that everything introduced by a package can be fully undone.

## Features
- Full removal of packages installed via pacman
- Tracking of changes for clean and reliable uninstalls
- Simple, familiar and Arch-focused design

---

## Why This Project?
Pacman is a powerful package manager, but sometimes uninstalling a package leaves behind residual files. These unused files waste disk space and are hard to trace, making full cleanup difficult.
 
If you're like me, you chose Arch Linux exactly because you want full control over your machine.

**unpacman** was created to explore whether it’s possible to go one step further: to provide a complete rollback mechanism, like pressing Ctrl+Z for your system.

---

## How It works?
Whenever you run a pacman command to install or update a package, the hooks system attaches metadata to every file, making them traceable even if the main package is later removed.
...

---

## Installation
> **Note:** This project is currently paused and not under active development.  

If you still want to try it out:

```bash
# Clone the repository
git clone https://github.com/marciomavungo/unpacman.git
cd unpacman

# Install dependencies
sudo pacman -S python-pip
pip install -r requirements.txt

# Create a hook
sudo mkdir -p /etc/pacman.d/hooks
cd /etc/pacman.d/hooks
...
```
---

## Contributing
Contributions are welcome. The project is currently paused, so changes may not be merged immediately.  
To contribute, fork the repository, make your changes in a branch, and open a Pull Request.

---

⚠️ **Project status:** paused — not under active development.