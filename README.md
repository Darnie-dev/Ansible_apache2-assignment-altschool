# Ansible_apache2-assignment-altschool# Automating Apache Installation and Configuration with Ansible

Hey there!

Welcome to my Ansible project for automating the installation and configuration of Apache HTTP Server on Debian and CentOS nodes. With this playbook, you can easily set up Apache, replace the default webpage with content from a GitHub repository, and ensure everything is up and running smoothly.

## Requirements

Before you get started, make sure you have the following:

- Ansible installed on your control node.
- SSH access to your Debian and CentOS servers.
- A list of server IP addresses or hostnames in your inventory file.
- The URL of your GitHub repository containing the webpage content you want to deploy.

## How to Use

1. **Clone the Repository**: Grab the code from this repository and save it to your local machine.

2. **Update Inventory**: Open up the `inventory_file` and add the IP addresses or hostnames of your target servers.

3. **Customize the Playbook**: Take a look at the `configure_apache.yml` playbook. You may need to update the GitHub repository URL to point to your own.

4. **Run the Playbook**: Fire up your terminal, navigate to the project directory, and run the playbook using:
   ```bash
   ansible-playbook -i inventory_file configure_apache.yml
