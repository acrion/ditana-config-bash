# Ditana Config Bash

This Arch Linux package provides bash-specific configurations for Ditana GNU/Linux, complementing the shared shell configurations.

## Description

Ditana Config Bash sets up bash-specific settings and integrations for Ditana GNU/Linux. It works in conjunction with the [ditana-config-shell](https://github.com/acrion/ditana-config-shell) package, which provides the common shell configurations shared between bash and zsh.

## Features

- Bash-specific configuration file (`.bashrc_ditana`)
- Integration with Starship prompt
- Automatic setup script to replace the default `.bashrc` with the Ditana-specific version

## Components

1. **`.bashrc_ditana`**:
   - Initializes [Starship prompt](https://starship.rs) for bash
   - Sources the common `.shellrc` file (provided by [ditana-config-shell](https://github.com/acrion/ditana-config-shell))

2. **`ditana-bash-setup.sh`**:
   - Automatically replaces the default `.bashrc` with `.bashrc_ditana` at first login
   - Ensures Ditana-specific bash configurations are applied without modifying `/etc/skel/.bashrc`, which is part of the [bash package](https://archlinux.org/packages/core/x86_64/bash).

## Installation

On Ditana GNU/Linux, this package is installed by default.

## Dependencies

- [ditana-config-shell](https://github.com/acrion/ditana-config-shell)
- [bash](https://archlinux.org/packages/core/x86_64/bash)
- [starship](https://gitlab.archlinux.org/archlinux/packaging/packages/starship)

## Usage

The Ditana bash configuration is automatically applied after installation. Users don't need to take any additional steps to activate it.

## Customization

For user-specific customizations:
1. Edit `~/.bashrc` for bash-specific settings
2. Use `~/.shellrc` or `~/.shell.d/` directory for configurations shared with zsh (see [ditana-config-shell](https://github.com/acrion/ditana-config-shell))

## Relation to ditana-config-shell

While this package provides bash-specific configurations, the majority of shell settings are managed by the [ditana-config-shell](https://github.com/acrion/ditana-config-shell) package. This separation allows for a clean, modular approach to shell configuration in Ditana GNU/Linux.

## Support

For issues, feature requests, or contributions related to Ditana Config Bash, please use the GitHub issue tracker or submit a pull request.

---

Ditana Config Bash is part of the Ditana GNU/Linux project, providing a tailored bash experience while maintaining consistency with the overall shell environment.
