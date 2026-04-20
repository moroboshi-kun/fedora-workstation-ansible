# ssh_keys

Generates ed25519 SSH keypairs for the configured list of identities.

## Variables

| Variable | Default | Description |
|---|---|---|
| `ssh_keys_user` | `USER` env var | Key owner |
| `ssh_keys_base_dir` | `~/.ssh` | Base directory for keys |
| `ssh_keys_list` | see defaults | List of `{path, comment}` entries |

## Notes

- Keys are never overwritten (`force: false`). Re-running is safe.
- After running, add the generated public keys to GitHub/GitLab before switching remotes to SSH.
