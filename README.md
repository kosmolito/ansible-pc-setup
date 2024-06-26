# Ansible PC Setup

## About

This repository contains a set of Ansible playbooks to setup a Fedora environment including installing dnf, flatpak packages and setup repofiles. This is a personal project and the aim is to automate the setup of a Fedora environment as much as possible.
The playbooks are designed to be idempotent and can be run multiple times without causing any issues.

## Requirements

- Fedora
- Ansible

## Usage

```bash
# Clone the repository using the following command
git clone https://github.com/kosmolito/ansible-pc-setup.git

# Change the directory to the cloned repository
cd ansible-pc-setup

# Install Ansible if it is not already installed
sudo dnf update -y && sudo dnf install -y ansible

# Install the required Ansible collections, if they are not already installed
ansible-galaxy collection install -r requirements.yml

# Run the playbooks.
ansible-playbook local.yml
```
