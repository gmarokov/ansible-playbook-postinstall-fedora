WIP: Ansible playbook: Post Fedora workstation installation 
=========
[![Build Status](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora.svg?branch=master)](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora)

Post Fedora installation Ansible script for provisioning dev machine.

## Installation
1. Install Ansible
`sudo dnf install ansible`
2. Add entry to your hosts in `/etc/ansible/hosts`:
```
[localhost] 
127.0.0.1
```

## Usage
`ansible-pull -U https://github.com/gmarokov/ansible-playbook-postinstall-fedora.git -e become-pass=your-sudo-pass`

## Script details 

### Pre tasks
- Update system

### Tasks

#### Install dnf packages
- Git
- CopyQ
- Gnome Tweaks

#### Install snap packages
- Visual Studio Code
- Postman
- .NET Core SDK 2.1
- Node.js 12
- Docker
- Firefox
- Spotify

### Post task
- Reboot
