# Ansible Apache Role

## Project Overview

This project demonstrates how to convert an existing Ansible playbook into a reusable Ansible role.

The role installs the Apache web server and deploys a custom `index.html` file to the target servers.

This project was created while learning Ansible from the **Ansible Zero to Hero** series by Abhishek Veeramalla.

## Features

* Install Apache web server
* Copy a custom `index.html` file to the web server
* Use an Ansible role for better project structure
* Execute the role using an Ansible playbook
* Configure multiple remote servers using Ansible

## Project Structure

```text
Ansible/
├── first-playbook.yaml
├── inventory.ini
└── test/
    ├── defaults/
    ├── files/
    │   └── index.html
    ├── handlers/
    ├── meta/
    ├── tasks/
    │   └── main.yml
    ├── templates/
    ├── tests/
    └── vars/
```

## Prerequisites

Before running this project, make sure you have:

* Ubuntu or Linux system
* Ansible installed
* Two or more remote servers
* SSH passwordless authentication configured
* Inventory file containing the target servers

## How to Run

Clone the repository:

```bash
git clone https://github.com/Preetham-Thyagarthy-S/ansible-apache-role.git
```

Go to the project directory:

```bash
cd ansible-apache-role
```

Run the playbook:

```bash
ansible-playbook -i inventory.ini first-playbook.yaml
```

## Expected Output

After the playbook runs successfully:

* Apache will be installed on all target servers.
* The custom `index.html` file will be copied to the Apache web directory.
* Opening the server's public IP in a browser will display the deployed web page.

## Technologies Used

* Ansible
* YAML
* Apache HTTP Server
* HTML
* Linux
* AWS EC2

## Learning Outcome

Through this project, I learned:

* Creating Ansible roles
* Organizing Ansible projects
* Using the `files` directory in roles
* Writing Ansible tasks
* Running playbooks using an inventory file
* Automating Apache installation and web page deployment

## Author

**Preetham Thyagarthy**

