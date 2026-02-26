<div align="center">

# asdf-roc [![Build](https://github.com/aotarola/asdf-roc/actions/workflows/build.yml/badge.svg)](https://github.com/aotarola/asdf-roc/actions/workflows/build.yml) [![Lint](https://github.com/aotarola/asdf-roc/actions/workflows/lint.yml/badge.svg)](https://github.com/aotarola/asdf-roc/actions/workflows/lint.yml)

[roc](https://www.roc-lang.org/docs) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `bash`, `curl`, `tar`, `git`, and [POSIX utilities](https://pubs.opengroup.org/onlinepubs/9699919799/idx/utilities.html).

# Install

Plugin:

```shell
asdf plugin add roc
# or
asdf plugin add roc https://github.com/aotarola/asdf-roc.git
```

roc:

```bash#ci
# Show all installable versions
asdf list-all roc

# Install specific version
asdf install roc latest

# Set a version globally (on your ~/.tool-versions file)
asdf global roc latest

# Now roc commands are available
roc version
```

You can also install the `nightly` version, which tracks the latest pre-release:

```bash#ci
asdf install roc nightly
```

Since asdf caches installed versions, you need to uninstall and reinstall to get the latest nightly:

```bash#ci
asdf uninstall roc nightly && asdf install roc nightly
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/aotarola/asdf-roc/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Andres Otarola](https://github.com/aotarola/)
