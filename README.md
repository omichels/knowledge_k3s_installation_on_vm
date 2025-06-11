## Installation of K3S on Virtual Maschine(s)


### Santiy settings on Red Hat

- disable SELINUX
- disable firewalld


curl -sfL https://get.k3s.io | INSTALL_K3S_SKIP_SELINUX_RPM=true INSTALL_K3S_SELINUX_WARN=true sh -



### Installation on second node


curl -sfL https://get.k3s.io | INSTALL_K3S_SKIP_SELINUX_RPM=true INSTALL_K3S_SELINUX_WARN=true K3S_URL=https://<server_ip>:6443 K3S_TOKEN=<node_token> sh

