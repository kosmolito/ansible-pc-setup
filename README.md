# Ansible Fedora Environment Setup

## About

This repository contains a set of Ansible playbooks to setup a Fedora environment including installing dnf, flatpak packages and setup repofiles. This is a personal project and the aim is to automate the setup of a Fedora environment as much as possible.
The playbooks are designed to be idempotent and can be run multiple times without causing any issues.

## Requirements

- Fedora
- Ansible

## Usage

```bash
# Clone the repository using the following command
git clone https://github.com/kosmolito/ansible-fedora-environment-setup.git

# Change the directory to the cloned repository
cd ansible-fedora-environment-setup

# Install Ansible if it is not already installed
sudo dnf update -y && sudo dnf install -y ansible

# Install the required Ansible collections, if they are not already installed
ansible-galaxy collection install -r requirements.yml

# Run the playbooks. -K flag is used to prompt for the sudo password
ansible-playbook -K playbook.yml
```
