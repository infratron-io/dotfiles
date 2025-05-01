## System Packages (via APT)

### Core System Utilities

- apt-transport-https
- ca-certificates
- gnupg
- lsb-release
- dialog
- build-essential
- curl
- wget
- time
- tree
- parallel
- file
- procps
- zip
- python3
- python3-venv
- dnsutils

### Development Tools

- git
- jq
- git-lfs (installed from GitHub releases)

### Container Tools

- docker-ce
- docker-ce-cli
- containerd.io
- docker-compose-plugin
- docker-buildx-plugin
- docker-compose (via GitHub releases)
- Docker credential helpers (secretservice for GNOME, wincred for WSL)

### Terminal Tools

- zsh (primary shell)
- asciinema (terminal recorder)

### Windows Subsystem for Linux (WSL) Tools

- wslu (when in WSL)

### Desktop Environment (when on Ubuntu Desktop with GNOME)

- yaru-theme-gtk
- yaru-theme-icon
- yaru-theme-sound
- yaru-theme-gnome-shell (when not in WSL)
- gnome-tweaks
- gnome-menus
- python3-nautilus
- libsecret-1-0 (when not in WSL)

### Window Manager

- Hyprland (if installation flag is set)
- mason (if Hyprland is installed)

### Applications (when on Ubuntu Desktop)

- Visual Studio Code (via Microsoft's APT repository)
- Google Chrome (via Google's APT repository)
- 1Password (via 1Password's APT repository)
- Spotify (via Spotify's APT repository)

### Authentication Tools

- Git Credential Manager (GCM)

### Linux Kernels (when not in WSL)

- linux-generic-hwe-22.04 (for Ubuntu 22.04 Jammy)
- linux-generic-hwe-20.04 (for Ubuntu 20.04 Focal)
- linux-generic-hwe-24.04 (for Ubuntu 24.04 Noble)

### Explicitly Uninstalled Packages

- gcmcore
- direnv (installed via chezmoi external instead)
- crudini
- fzf (installed via chezmoi external instead)
- docker-scan-plugin (deprecated)
- pipx (installed via chezmoi external instead)

The dotfiles setup adds several APT repositories:

- Docker
- Git Core PPA
- Visual Studio Code
- Google Chrome
- 1Password
- Spotify
- Hyprland (if installation flag is set)
- WSLU PPA (when in WSL)

This system-level installation complements the user-level installations seen earlier, with core system packages and desktop applications installed system-wide through APT, while development tools and utilities are primarily installed at the user level through various package managers.
