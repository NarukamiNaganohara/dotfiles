# My Dotfiles Repository

## Welcome

Hello! 👋 Welcome to my personal dotfiles repository. This is a collection of configuration files (dotfiles) for my Linux setup, primarily based on Arch Linux with Hyprland as the window manager. These configs customize tools like my terminal, file manager, prompt, and desktop environment to suit my workflow. Feel free to browse, get inspired, or fork it—but read the warnings below before using anything!

This repo includes configs for a rice'd (customized) setup with themes, keybindings, and utilities for productivity and aesthetics. It's a work in progress, and I'm sharing it to document my setup.

## Required Packages and Tools

Here are the key packages and tools used in this dotfiles setup. I've included links to their official documentation for installation and configuration details. These are the core ones; others like btop, cava, fastfetch, etc., are also configured but not exhaustive.

- **Yazi**: A fast, extensible file manager for the terminal.  
  [Official Documentation](https://yazi-rs.github.io/docs/)

- **Neovim (nvim)**: A highly configurable text editor for efficient coding and writing.  
  [Official Documentation](https://neovim.io/doc/)

- **Kitty**: A fast, feature-rich, GPU-accelerated terminal emulator.  
  [Official Documentation](https://sw.kovidgoyal.net/kitty/)

- **Starship**: A minimal, blazing-fast, and customizable prompt for any shell.  
  [Official Documentation](https://starship.rs/guide/)

- **Hyprland**: A dynamic tiling Wayland compositor with smooth animations and customizability.  
  [Official Documentation](https://wiki.hyprland.org/)

- **Fish**: A smart and user-friendly command-line shell.  
  [Official Documentation](https://fishshell.com/docs/current/)

- **Lazygit**: A simple terminal UI for Git commands.  
  [Official Documentation](https://github.com/jesseduffield/lazygit/wiki)

- **Mako**: A lightweight Wayland notification daemon.  
  [Official Documentation](https://github.com/emersion/mako/wiki)

- **Wofi**: A launcher/menu program for Wayland.  
  [Official Documentation](https://hg.sr.ht/~scoopta/wofi)

- **Fastfetch**: A neofetch-like tool for fetching system information with speed.  
  [Official Documentation](https://github.com/fastfetch-cli/fastfetch/wiki)

- **NWG-Look**: A tool for customizing GTK themes on Wayland.  
  [Official Documentation](https://github.com/nwg-piotr/nwg-look/wiki)

- **Qt5ct**: A Qt5 configuration tool for theming.  
  [Official Documentation](https://sourceforge.net/projects/qt5ct/)

- **Kvantum**: A SVG-based theme engine for Qt.  
  [Official Documentation](https://github.com/tsujan/Kvantum/wiki)

- **Btop**: An advanced system monitor for the terminal.  
  [Official Documentation](https://github.com/aristocratos/btop/wiki)

- **Cava**: A console-based audio visualizer.  
  [Official Documentation](https://github.com/karlstav/cava/wiki)

Other tools like Goverlay, MangoHud, vkBasalt, MPV, and more are included for gaming/graphics tweaks, but check their respective repos for docs.

## Warnings

⚠️ **Do not copy these dotfiles directly into your own setup!** This is my personal configuration, tailored to my hardware and preferences. Blindly copying could break your system or cause unexpected behavior.

- Specifically, in the Hyprland configs (`hypr/` directory), there are potential issues or "errors" (as in, unoptimized parts) related to monitor setup. You **must** adjust the monitor configurations (e.g., resolutions, positions, and outputs) to match your own hardware. The same goes for Hyprlock (screen locker) and wallpaper settings—they rely on specific paths and themes that might not exist on your system.

- Always back up your existing configs before testing anything. Test in a virtual machine if possible.

- Some configs assume Arch Linux with AUR access (via yay), so compatibility on other distros may vary.

## Installation Commands for Different Linux Distributions

Below are example installation commands for the key tools on popular Linux distributions. **These are not exhaustive or guaranteed to work—always refer to the official documentation links above for the most up-to-date instructions.** I strongly recommend installing manually by studying the specific docs for each tool, as package names, dependencies, and versions can differ. Automated scripts can miss edge cases or introduce security risks.

### Arch Linux (using pacman and AUR via yay)

- Yazi: `yay -S yazi` (or build from source per docs)
- Neovim: `sudo pacman -S neovim`
- Kitty: `sudo pacman -S kitty`
- Starship: `sudo pacman -S starship`
- Hyprland: `sudo pacman -S hyprland` (see wiki for full setup)
- Fish: `sudo pacman -S fish`
- Lazygit: `sudo pacman -S lazygit`
- Mako: `sudo pacman -S mako`
- Wofi: `sudo pacman -S wofi`
- Fastfetch: `yay -S fastfetch`
- For others, check AUR or pacman repos.

Official Arch docs: [Arch Wiki](https://wiki.archlinux.org/)

### Debian/Ubuntu (using apt)

- Neovim: `sudo apt install neovim` (or use PPA for latest)
- Kitty: `sudo apt install kitty`
- Starship: `curl -sS https://starship.rs/install.sh | sh` (per docs)
- Fish: `sudo apt install fish`
- Lazygit: Use snap or build from source (see docs)
- Others like Hyprland may require building from source or PPAs, as Wayland support varies.

Official Ubuntu docs: [Ubuntu Documentation](https://ubuntu.com/tutorials)

### Fedora (using dnf)

- Neovim: `sudo dnf install neovim`
- Kitty: `sudo dnf install kitty`
- Starship: `curl -sS https://starship.rs/install.sh | sh`
- Fish: `sudo dnf install fish`
- Hyprland: Available in COPR repos—see Hyprland docs for setup.
- Others: Check Fedora repos or build.

Official Fedora docs: [Fedora Project Wiki](https://docs.fedoraproject.org/)

### openSUSE (using zypper)

- Neovim: `sudo zypper install neovim`
- Kitty: `sudo zypper install kitty`
- Starship: Install via script per docs.
- Fish: `sudo zypper install fish`
- Others: Use OBS (open Build Service) for packages not in main repos.

Official openSUSE docs: [openSUSE Wiki](https://en.opensuse.org/Portal:Documentation)

**Warning:** For all distros, Wayland-based tools like Hyprland require compatible hardware/drivers. Always verify compatibility and update your system first. Manual installation from source is often best for cutting-edge features.

## Acknowledgments

This setup draws inspiration from key people and technologies in the Linux community:

- **Hyprland developers** (e.g., Vaxry) for revolutionizing Wayland compositing.
- **Neovim core team** for maintaining an extensible editor.
- **Starship contributors** for a cross-shell prompt that's both beautiful and functional.
- Open-source pioneers like the Fish shell team, and communities around Arch, Wayland, and ricing.

Special thanks to the broader FOSS community for tools like these!

Thank you for visiting this repository! If you find it useful, star it or open an issue with suggestions. Happy configuring! 🚀
kvantum qt5ct nwg-look mangohud goverlay vkbasalt
