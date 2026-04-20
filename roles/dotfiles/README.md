# dotfiles

Deploys dotfiles from a local clone of the dotfiles repository.

## Variables

| Variable | Default | Description |
|---|---|---|
| `dotfiles_repo_path` | `~/Development/github/moroboshi/dot_files` | Path to the dotfiles repo clone |
| `dotfiles_user` | `USER` env var | Owner for deployed files |
| `dotfiles_distro` | `fedora` | Selects the distro-specific bashrc variant (`bash/<distro>/bashrc`) |

## Prerequisites

The dotfiles repository must already be cloned at `dotfiles_repo_path` before this role runs. The `bootstrap.sh` script handles this.
