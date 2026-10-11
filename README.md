# FMOS package repository

The live `[fmos]` pacman repository is served from the **`gh-pages` branch**
of this repo: https://fmos-linux.github.io/packages/

## Usage

    # /etc/pacman.conf
    [fmos]
    SigLevel = Required
    Server = https://fmos-linux.github.io/packages/

Install the keyring first — `fmos-keyring` (from this repo), or see
[fmos-linux/keyring](https://github.com/fmos-linux/keyring) for manual trust.

## Contents

- The FMOS suite (`fmos-*`: desktop meta, hyprland configs, branding,
  hyprpanel, welcome/firstrun, update/restore).
- The pinned AGS/Astal chain (`aylurs-gtk-shell-git`, `libastal-*`,
  `quarrel-git`, `libcava`, `appmenu-glib-translator-git`) that
  `fmos-hyprpanel` needs — built from the FMOS source mirrors.

Everything is GPG-signed (see [fmos-linux/keyring](https://github.com/fmos-linux/keyring)).
PKGBUILDs live in the FMOS monorepo until the org split; this branch carries
only build artifacts.
