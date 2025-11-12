# ansible-docker-lab

# 🐳 Ansible Docker Lab

This project automates the installation of Docker and the deployment of a containerized Nginx web app using Ansible.

---

## 🚀 Features
- Installs Docker CE on Ubuntu/Debian  
- Deploys an Nginx container  
- Mounts a custom HTML page inside the container  
- Automatically restarts container if stopped  

---

## 🧭 How to Run

1. Edit your inventory:
   `ini
   [servers]
   localhost ansible_connection=local

2. Run the playbook:

ansible-playbook playbooks/site.yml


3. Open your browser:

http://localhost

You should see your custom message!




---

🧠 Roles

Role Description

docker Installs and configures Docker
nginx_container Runs an Nginx container with a mounted HTML page



---
---
ansible-docker-lab/
│
├── ansible.cfg
├── README.md
│
├── inventory/
│   └── hosts.ini
│
├── playbooks/
│   └── site.yml
│
└── roles/
    ├── docker/
    │   └── tasks/main.yml
    │
    ├── nginx_container/
    │   ├── tasks/main.yml
    │   ├── templates/index.html.j2
    │   └── vars/main.yml

---
🧑‍💻 Author: Meisam Amiri

Linux System Administrator / DevOps Engineer
