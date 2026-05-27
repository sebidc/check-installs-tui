<img width="967" height="597" alt="image" src="https://github.com/user-attachments/assets/3de5c9e7-3f73-497c-858e-9c63ea774273" />

# check installs TUI

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Release](https://img.shields.io/github/v/release/sebidc/check-installs-tui?display_name=tag)](https://github.com/sebidc/check-installs-tui/releases)
[![Platform](https://img.shields.io/badge/platform-macOS%20Terminal-111827)](https://github.com/sebidc/check-installs-tui)
[![Homebrew Tap](https://img.shields.io/badge/homebrew-sebidc%2Ftap-fbbf24)](https://github.com/sebidc/homebrew-tap)

`check-installs-tui` is a macOS terminal dashboard for browsing packages installed across common developer package managers. It scans your local tools, groups installs by manager, shows package metadata, and gives you a fast keyboard-and-mouse interface for searching what is on your machine.

## What's New in v1.0.0

This release promotes the newer dashboard experience that was added after the early `v0.1.0-alpha` line:

- Full-screen curses dashboard with package list, search, package details, and manager distribution graph.
- Animated loading screen that reports the manager currently being scanned, such as `loading brew packages` or `loading npm packages`.

<img width="967" height="597" alt="image" src="https://github.com/user-attachments/assets/d5ab4dbd-e585-4937-af56-7df6991acdfc" />

- Progress details below the loading bar so the bar stays clean and readable.
- Mouse wheel and keyboard navigation for package rows and detail popups.
- Selection popup with copy actions for package fields.
- Path popup with copy/open/reveal actions for installed package locations.
- Homebrew installs a short `ci` command alongside `check-installs-tui`.

## Supported Managers

`check-installs-tui` detects whichever of these tools are available on your Mac:

- `brew`
- `npm`
- `pnpm`
- `yarn`
- `bun`
- `pipx`
- `pip3`
- `cargo`
- `gem`
- `mas`

Missing managers are skipped automatically.

## Install

### Homebrew

```sh
brew tap sebidc/tap
brew install check-installs-tui
```

## Usage

Run the full command:

```sh
check-installs-tui
```

Or use the short Homebrew shortcut:

```sh
ci
```

## Controls

- Type to search packages.
- Use `Up`/`Down`, `j`/`k`, or the mouse wheel to move through results.
- Press `Enter` on a package to open the selection popup.
- Use the path popup to copy, open, or reveal an install location.
- Press `q` or `Esc` to close popups or quit.

## Interface

The dashboard is split into a package list and a detail sidebar. The top dashboard summarizes host, shell, total packages, detected managers, disk usage, and manager distribution. The right panel shows the selected package fields and a manager-level graph.

## Repository

- [Contributing](./CONTRIBUTING.md)
- [Security](./SECURITY.md)
- [MIT License](./LICENSE)
