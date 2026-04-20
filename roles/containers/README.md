# containers

Installs podman and podman-compose.

## Variables

| Variable | Default | Description |
|---|---|---|
| `containers_packages` | `[podman, podman-compose]` | Packages to install |

## Notes

- Podman is daemonless — no service management or group membership required.
- Both packages are available in the default Fedora repos.
