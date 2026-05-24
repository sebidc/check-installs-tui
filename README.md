# check installs TUI

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Release](https://img.shields.io/github/v/release/sebidc/check-installs-tui?display_name=tag)](https://github.com/sebidc/check-installs-tui/releases)
[![Platform](https://img.shields.io/badge/platform-macOS%20Terminal-111827)](https://github.com/sebidc/check-installs-tui)
[![Homebrew Tap](https://img.shields.io/badge/homebrew-sebidc%2Ftap-fbbf24)](https://github.com/sebidc/homebrew-tap)

`check-installs-tui` is a terminal UI for browsing packages installed through common macOS package managers.

Supported managers include:

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

## Install

### Homebrew

```sh
brew tap sebidc/tap
brew install check-installs-tui
```

## Usage

```sh
check-installs-tui
```

Layout:

1. Packages
2. Dashboard
3. Search

The right panel shows package details and a manager-level graph for the selected row.

## Repository

- [Contributing](./CONTRIBUTING.md)
- [Security](./SECURITY.md)
- [MIT License](./LICENSE)
