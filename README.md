# asdf-act

[![Build](https://github.com/gr1m0h/asdf-act/actions/workflows/build.yaml/badge.svg)](https://github.com/gr1m0h/asdf-act/actions/workflows/build.yaml)
[![Lint](https://github.com/gr1m0h/asdf-act/actions/workflows/lint.yaml/badge.svg)](https://github.com/gr1m0h/asdf-act/actions/workflows/lint.yaml)

[act](https://github.com/nektos/act) plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

```shell
asdf plugin add act https://github.com/gr1m0h/asdf-act.git
```

## Usage

See the [asdf documentation](https://asdf-vm.com/manage/core.html) for the full
set of commands. The most common ones are:

```shell
# Show all installable versions
asdf list all act

# Install a specific version
asdf install act latest
asdf install act 0.2.80

# Set a version globally (writes to ~/.tool-versions)
asdf set -u act latest

# Set a version for the current project (writes to ./.tool-versions)
asdf set act 0.2.80
```

## Contributing

Contributions are welcome! This plugin is linted with
[shellcheck](https://www.shellcheck.net/) and
[shfmt](https://github.com/mvdan/sh), and tested with
[asdf-vm/actions](https://github.com/asdf-vm/actions).

The required tooling versions are pinned in [`.tool-versions`](./.tool-versions),
so you can install them with asdf:

```shell
asdf install
```

```shell
# Format the shell scripts
./scripts/format.bash

# Lint the shell scripts
./scripts/lint.bash
```

## License

[MIT](./LICENSE)
