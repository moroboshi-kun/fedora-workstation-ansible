# kubernetes

Adds the Kubernetes dnf repository, installs kubectl, and installs the minikube binary.

## Variables

| Variable | Default | Description |
|---|---|---|
| `kubernetes_kubectl_repo_name` | `kubernetes` | Repo name |
| `kubernetes_kubectl_repo_baseurl` | pkgs.k8s.io v1.35 | Repo base URL |
| `kubernetes_kubectl_repo_gpgkey` | pkgs.k8s.io v1.35 | GPG key URL |
| `kubernetes_minikube_version` | `v1.38.1` | Minikube release to install |
| `kubernetes_minikube_dest` | `/usr/local/bin/minikube` | Install path |
