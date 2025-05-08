<div align="center">


# asdf-watchman
[![Build](https://github.com/CodiAsFox/asdf-watchman/actions/workflows/build.yml/badge.svg)](https://github.com/CodiAsFox/asdf-watchman/actions/workflows/build.yml)
[![Lint](https://github.com/CodiAsFox/asdf-watchman/actions/workflows/lint.yml/badge.svg)](https://github.com/CodiAsFox/asdf-watchman/actions/workflows/lint.yml)

An [asdf](https://asdf-vm.com) plugin for installing [Watchman](https://facebook.github.io/watchman/), a file watching service developed by Facebook.

</div>

---

## Contents

- [asdf-watchman](#asdf-watchman)
  - [Contents](#contents)
  - [Dependencies](#dependencies)
    - [macOS](#macos)
    - [Linux](#linux)
  - [Install](#install)
  - [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Dependencies

This plugin builds Watchman from source. You will need:

### macOS

- [Homebrew](https://brew.sh)
- `cmake`, `autoconf`, `automake`, `libtool`, `pcre`, `pkg-config`

```sh
brew install cmake autoconf automake libtool pcre pkg-config
```

### Linux

- Install the following using your package manage (e.g., apt, dnf, or pacman):
-	cmake, autoconf, automake, libtool, pkg-config, pcre (plus dev headers)

Example (Debian/Ubuntu):

```sh
sudo apt update
sudo apt install -y cmake autoconf automake libtool pkg-config libpcre3-dev
```
---

## Install

Add plugin:

```sh
asdf plugin add watchman https://github.com/CodiAsFox/asdf-watchman.git
```

Install watchman:

```sh
# List available versions
asdf list-all watchman

# Install a specific version (must be v2021+)
asdf install watchman 2023.09.25.00

# Set it globally
asdf global watchman 2023.09.25.00

# Verify
watchman --version
```

---

## Usage

This plugin supports Watchman versions 2021+ only. Older versions using autogen.sh are not supported due to incompatibility with the modern CMake build system.

---

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/CodiAsFox/asdf-watchman/graphs/contributors)!

---

# License

See [LICENSE](LICENSE) © [Taylor Jay Fox](https://github.com/CodiAsFox/)

Forked from [Jeppe Kristensen](https://github.com/jepify/asdf-watchman)