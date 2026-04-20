# dev_tools

Installs development tools via dnf.

## Variables

| Variable              | Default | Description                    |
|-----------------------|---------|--------------------------------|
| `dev_tools_packages`  | see defaults | List of dev packages to install |

## Notes

- `opentofu` requires the opentofu repo to be available. Add it to the `packages` role or a dedicated `repos` role if needed.
- `glab` may not be in the default Fedora repos; verify availability or add a COPR.
