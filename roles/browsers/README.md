# browsers

Adds the Brave browser RPM repository and installs browsers and mail client.

## Variables

| Variable | Default | Description |
|---|---|---|
| `browsers_brave_gpg_key` | brave-core.asc URL | GPG key for Brave repo |
| `browsers_brave_repo_baseurl` | brave x86_64 URL | Brave repo base URL |
| `browsers_packages` | `[brave-browser, thunderbird]` | Packages to install |
