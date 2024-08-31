# Automated Installation of Java and MySQL on AWS EC2

## Overview

This project demonstrates the use of Ansible to automate the installation of Java and MySQL on AWS EC2 instances using a single playbook. 
The playbook is designed to run on multiple nodes, with conditional tasks based on the host.

## Setup

1. **Create EC2 Instances:**
   - One instance as the Ansible Master.
   - Two instances as Ansible Slave.

2. **Install Ansible:**
   - Install Ansible on the Ansible Master.

3. **Configure Inventory File:**
   - Update the `inventory` file with the IP addresses of your Ansible Slaves.

4. **Run the Playbook:**
   ```bash
   ansible-playbook -i inventory playbook.yml
