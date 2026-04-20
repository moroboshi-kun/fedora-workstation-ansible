# fedora-workstation-ansible

Ansible project for configuring a Fedora 43 workstation.

## Quick start (fresh machine)

```bash
curl -fsSL https://raw.githubusercontent.com/moroboshi-kun/fedora-workstation-ansible/main/bootstrap.sh | bash
```

Or clone manually and run:

```bash
sudo dnf install -y git ansible python3
git clone https://github.com/moroboshi-kun/fedora-workstation-ansible.git
cd fedora-workstation-ansible
ansible-galaxy collection install -r requirements.yml
ansible-playbook site.yml --ask-become-pass
```

## Running specific roles

```bash
ansible-playbook site.yml --tags packages
ansible-playbook site.yml --tags containers,kubernetes
```

## Roles

| Role | Description |
|---|---|
| `packages` | Base system packages via dnf |
| `dev_tools` | Development tools via dnf |
| `containers` | Docker, docker-compose, docker group membership |
| `kubernetes` | kubectl (via k8s repo) and minikube binary |
| `browsers` | Brave browser repo + Thunderbird |
| `fonts` | SauceCodePro Nerd Font |
| `dotfiles` | Deploys dotfiles from local repo clone |
| `ssh_keys` | Generates ed25519 SSH keypairs |
| `nvm` | NVM + pinned Node.js version |
| `powerline` | powerline-status + powerline-gitstatus via pipx |

## Development

```bash
pip install ansible ansible-lint molecule molecule-plugins[docker]
ansible-galaxy collection install -r requirements.yml

# Lint
ansible-lint

# Test a role
cd roles/ssh_keys && molecule test
```
