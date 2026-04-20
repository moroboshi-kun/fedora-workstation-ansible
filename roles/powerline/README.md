# powerline

Installs powerline-status and powerline-gitstatus via pipx.

## Variables

| Variable | Default | Description |
|---|---|---|
| `powerline_package` | `powerline-status` | Main pipx package |
| `powerline_inject_packages` | `[powerline-gitstatus]` | Packages to inject into the pipx venv |
| `powerline_pipx_executable` | `/usr/bin/pipx` | Path to pipx binary |

## Prerequisites

`python3-pipx` must be installed (handled by the `packages` role).
