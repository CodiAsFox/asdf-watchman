<div align="center">

# asdf-watchman [![Build](https://github.com/jepify/asdf-watchman/actions/workflows/build.yml/badge.svg)](https://github.com/jepify/asdf-watchman/actions/workflows/build.yml) [![Lint](https://github.com/jepify/asdf-watchman/actions/workflows/lint.yml/badge.svg)](https://github.com/jepify/asdf-watchman/actions/workflows/lint.yml)

[watchman](https://github.com/jepify/watchman) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

**TODO: adapt this section**

- `bash`, `curl`, `tar`: generic POSIX utilities.
- `SOME_ENV_VAR`: set this environment variable in your shell config to load the correct version of tool x.

# Install

Plugin:

```shell
asdf plugin add watchman
# or
asdf plugin add watchman https://github.com/jepify/asdf-watchman.git
```

watchman:

```shell
# Show all installable versions
asdf list-all watchman

# Install specific version
asdf install watchman latest

# Set a version globally (on your ~/.tool-versions file)
asdf global watchman latest

# Now watchman commands are available
watchman version
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/jepify/asdf-watchman/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Jeppe Kristensen](https://github.com/jepify/)
