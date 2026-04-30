# Ansible Multi-Node Setup

## Description
This project demonstrates how to configure multiple EC2 instances using Ansible.

## Architecture
- Control Node: Ansible server
- Target Nodes:
  - 1 Master node
  - 1 Worker node

## Features
- SSH-based communication
- Inventory-based host grouping
- Role-based configuration
- Automated package installation

## Technologies Used
- Ansible
- AWS EC2
- Linux (Ubuntu)

## Project Structure
- inventory → contains target server IPs
- playbook.yml → main execution file
- roles/master → tasks for master node
- roles/worker → tasks for worker nodes

## How to Run
1. Update inventory with target IPs
2. Ensure SSH access is configured
3. Run:
   ansible-playbook playbook.yml
