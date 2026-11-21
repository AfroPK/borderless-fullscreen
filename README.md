<p align="center">
  <img src=".github/assets/header.png" alt="Borderless Fullscreen: windowed apps · fullscreen" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/%7B%20linux%20%7D-D6246E?style=for-the-badge&labelColor=0B0608" alt="{ linux }">
  <img src="https://img.shields.io/badge/shell-0B0608?style=for-the-badge&labelColor=0B0608" alt="shell">
  <img src="https://img.shields.io/badge/xorg%20%2B%20wayland-0B0608?style=for-the-badge&labelColor=0B0608" alt="xorg + wayland">
  <img src="https://img.shields.io/badge/status-stable-D6246E?style=for-the-badge&labelColor=0B0608" alt="status: stable">
</p>

<p><img src=".github/assets/section-about.png" alt="01 About" width="100%"></p>

**`{ borderless-fullscreen }`**: a shell script that forces a windowed app into borderless fullscreen on Linux.

Some games only offer "windowed" or "exclusive fullscreen", and both are annoying on a multi-monitor desk. This puts the window you pick fullscreen without the mode switch, so alt-tab stays instant. It's the Linux take on the Borderless Gaming app from Windows.

> [!NOTE]
> Needs Xorg or Wayland tooling installed first — `xdotool` + `zenity` on Xorg, `wlr-randr` + `wmctrl` + `zenity` on Wayland. The installer asks which one you're on.

<p><img src=".github/assets/section-requirements.png" alt="02 Requirements" width="100%"></p>

| Session | Packages |
|---|---|
| Xorg | `xdotool` · `zenity` |
| Wayland | `wlr-randr` · `wmctrl` · `zenity` |

<p><img src=".github/assets/section-setup.png" alt="03 Setup" width="100%"></p>

**Needs:** `git` · `zenity` · `xdotool` or `wlr-randr` + `wmctrl`

```sh
# Debian/Ubuntu — Xorg
sudo apt-get install xdotool zenity
# Debian/Ubuntu — Wayland
sudo apt-get install wlr-randr wmctrl zenity
# Fedora — Xorg
sudo dnf install xdotool zenity
# Fedora — Wayland
sudo dnf install wlr-randr wmctrl zenity
# Arch — Xorg
pacman -Syu xdotool zenity
# Alpine — Xorg
apk add --upgrade xdotool zenity
```

1. Clone the repo and enter it: `git clone https://github.com/AfroPK/borderless-fullscreen.git && cd borderless-fullscreen`
2. `sudo chmod +x install.sh`
3. `sudo ./install.sh` and pick Wayland or Xorg.
4. It shows up in your application menu — launch it from there.

<p><img src=".github/assets/section-usage.png" alt="04 Usage" width="100%"></p>

Start the app, pick the window you want, and it goes borderless fullscreen. To remove it, run `sudo ./uninstall.sh` from the cloned repo.

<p><img src=".github/assets/section-notes.png" alt="05 Notes" width="100%"></p>

- Tested on Xorg and Wayland sessions; a few compositors handle window sizing differently.
- Inspired by [Borderless Gaming](https://github.com/Codeusa/Borderless-Gaming) on Windows.
- MIT licence.

<p align="center">
  <img src=".github/assets/footer.png" alt="play games · make games" width="100%">
</p>
