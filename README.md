# Ubuntu XFCE Server Orchestration

This repository contains Ansible playbooks for automating the setup and configuration of Ubuntu servers with XFCE desktop environment.

## Components

- **XFCE Desktop**: Lightweight desktop environment setup
- **XRDP**: Remote desktop protocol server
- **System Configurations**: 
  - UFW firewall rules
  - User management
  - SSL certificates
  - Remote access settings

## Usage

1. Clone this repository
2. Ensure Ansible is installed
3. Update the variables in `group_vars/all.yml` if needed
4. Run the master playbook:
   ```bash
   ansible-playbook master.yml
   ```

## Default Configuration

- XRDP port: 3389
- Default user password: 12345678 (change this after setup)
- Enabled ports: 80, 443, 3389, 3000, 4000, 8080

## Post-Installation

1. Change the default user password
2. Access the server using any RDP client
3. Configure additional XFCE settings as needed

