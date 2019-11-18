WIP: Ansible playbook: Post Fedora workstation installation 
=========
[![Build Status](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora.svg?branch=master)](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora)
Post Fedora installation Ansible script for provisioning dev machine.

## Installation
3. Install Ansible
5. Add `[local] 127.0.0.1` to your hosts in `/etc/ansible/hosts`

## Usage
`ansible-pull -U https://github.com/gmarokov/ansible-playbook-postinstall-fedora.git`

## Script details 

### Pre tasks
- Update system
