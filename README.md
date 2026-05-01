# 🚀 DevOps Automated Workstation (Ansible-Based Setup)

A fully automated DevOps environment setup using **Ansible** to configure a lightweight Linux workstation with essential DevOps tools in a single command.

This project is designed for **DevOps Automated workstation**.

---

# 🧠 Overview

This project automates the setup of a complete DevOps development environment including:

- Infrastructure as Code tools (Terraform, Vagrant)
- Virtualization (VirtualBox)
- Cloud CLI (AWS CLI)
- Development tools (VS Code, Git)
- Networking utilities
- Productivity tools (Brave Browser, OnlyOffice)

---

# ⚙️ Tech Stack

- Ansible (Automation Engine)
- Linux (Xubuntu Host)
- VirtualBox (Virtualization)
- Terraform (Infrastructure as Code)
- Vagrant (VM Automation)
- AWS CLI (Cloud Access)

---

# 📦 Installed Tools

✔ Git  
✔ Curl / Wget  
✔ Vim / Htop  
✔ Net-tools  
✔ DNS utilities  
✔ Traceroute  
✔ Nmap  
✔ Terraform  
✔ Vagrant  
✔ VirtualBox  
✔ AWS CLI v2  
✔ Visual Studio Code  
✔ Brave Browser  
✔ OnlyOffice  

---

# 🏗️ Architecture

```mermaid id="arch02"
graph TD;

A[Host Machine - Xubuntu Dell E7440] --> B[Ansible Playbook Automation]

B --> C1[Terraform]
B --> C2[Vagrant]
B --> C3[VirtualBox]
B --> C4[AWS CLI]

C3 --> D[Virtual Machines]

D --> E1[Docker Runtime Inside VM]
D --> E2[Jenkins CI/CD Server]
D --> E3[Grafana + Prometheus Monitoring]
🔄 Features
⚡ One-command full setup
🔁 Idempotent (safe to re-run anytime)
🧩 Auto dependency handling
🛠️ VirtualBox kernel module auto-fix
☁️ Cloud-ready CLI environment
💻 Lightweight host optimization
🚀 How to Use
1. Clone repository
git clone https://github.com/muhammadkamrankabeer-oss/devops-workstation-automation.git
cd devops-workstation-automation
2. Run playbook
ansible-playbook -i inventory setup.yml --ask-become-pass
📌 Learning Outcomes
Infrastructure automation using Ansible
Linux system provisioning
DevOps toolchain setup
Virtualization management
Cloud CLI integration
Real-world system automation
🧠 Future Improvements
Add Docker VM environment
Add Jenkins CI/CD pipeline
Add Prometheus + Grafana monitoring stack
Convert into full Ansible roles structure
Integrate Terraform cloud provisioning
👨‍💻 Author

Muhammad Kamran Kabeer

DevOps Learner | Linux Enthusiast | Automation Explorer

⭐ Support

If you like this project:

Give it a ⭐ on GitHub
Fork it and improve it
Share it on LinkedIn
