# Ansible Server Automation

This repository contains Ansible playbooks and roles for automating common Linux server administration tasks.

## Overview

The project follows a role-based Ansible structure to improve reusability, maintainability, and organization of automation code.

Automated tasks include:

- Nginx installation and configuration
- Docker installation and configuration
- Linux user provisioning
- System package updates

## Repository Structure

ansible-server-automation

inventory/
├── dev
├── prod
└── hosts

group_vars/
└── all.yml

playbooks/
├── site.yml
├── webserver.yml
├── docker.yml
├── create-user.yml
└── system-update.yml

roles/
├── nginx
├── docker
└── common

## Roles

### Nginx

- Install Nginx
- Start and enable the Nginx service

### Docker

- Install Docker
- Start and enable the Docker service
- Configure Docker group membership

### Common

- Shared automation tasks
- Reusable configuration components

## Features

- Role-based Ansible design
- Centralized variable management
- Environment-based inventory structure
- Reusable automation workflows
- Linux server administration automation

## Technologies Used

- Ansible
- Linux
- Nginx
- Docker
- Git
- GitHub

## Example Usage

ansible-playbook playbooks/site.yml

## Future Enhancements

- Additional reusable roles
- Environment-specific variables
- Application deployment automation
- Monitoring and logging automation
