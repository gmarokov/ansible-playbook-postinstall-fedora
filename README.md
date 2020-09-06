Ansible playbook: Post Fedora workstation installation 
=========
[![Build Status](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora.svg?branch=master)](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora)

Post Fedora installation Ansible script for provisioning dev machine.

## Installation
1. Install Ansible:
`sudo dnf install ansible`

2. Add entry localhost to your ansible hosts:
```
cat <<EOT >> /etc/ansible/hosts
[localhost] 
127.0.0.1
EOT
```
3. Become root:
`sudo -i`

## Usage
1. Run the following command to pull and run the playbook: `ansible-pull -U https://github.com/gmarokov/ansible-playbook-postinstall-fedora.git`

## Script details 

### Pre tasks
- Update system

### Tasks

#### Install dnf packages
- RPM Fusion repositories
- Git
- Gnome Tweaks
- GPaste
- Open Weather
- Chromium
- Snap
- VLC
- Mega sync

#### Install snap packages
- Postman
- Dbeaver
- Node.js latest
- Docker
- Dotnet SDK latest
- Visual Studio Code
- Spotify

