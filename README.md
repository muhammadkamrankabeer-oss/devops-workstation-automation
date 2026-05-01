# 🚀 DevOps Automated Workstation (Ansible-Based Setup)

A fully automated **DevOps base environment** built using Ansible to provision a lightweight Linux workstation with essential DevOps tools in a single command.

This project is designed for **DevOps automation **.

---

# 🧠 Overview

This project automates the setup of a complete DevOps development environment including:

- Infrastructure as Code tools (Terraform, Vagrant)
- Virtualization (VirtualBox)
- Cloud CLI (AWS CLI)
- Development tools (VS Code, Git)
- Networking utilities
- Browser and productivity tools

---

# ⚙️ Tech Stack

- Ansible (Automation)
- VirtualBox (VM management)
- Terraform (Infrastructure as Code)
- Vagrant (VM automation)
- AWS CLI (Cloud interaction)
- Linux (Xubuntu host system)

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


Host Machine (Xubuntu)
│
├── Ansible Playbook (Automation Engine)
│
├── DevOps Tools Installed on Host:
│ ├── Terraform
│ ├── Vagrant
│ ├── VirtualBox
│ ├── AWS CLI
│ ├── VS Code
│
└── Virtual Machines (via VirtualBox)
└── Docker / Jenkins / Grafana (inside VM)


---

# 🔄 Features

- ⚡ One-command full setup
- 🔁 Idempotent (safe to re-run)
- 🧩 Auto dependency handling
- 🛠️ VirtualBox kernel auto-fix (vboxdrv issue handling)
- ☁️ Cloud-ready CLI setup
- 💻 Lightweight host optimization

---

# 🚀 How to Use

### 1. Clone repository
```bash
git clone https://github.com/your-username/devops-workstation.git
cd devops-workstation
2. Run playbook
ansible-playbook -i inventory setup.yml --ask-become-pass
📌 Learning Outcomes
Infrastructure automation using Ansible
Linux system provisioning
DevOps toolchain setup
Virtualization management
Cloud CLI integration
🧠 Future Improvements
Add Docker VM environment
Add Jenkins + CI/CD pipeline
Add Prometheus + Grafana monitoring stack
Convert into Ansible roles structure
Integrate Terraform provisioning
👨‍💻 Author

Muhammad Kamran Kabeer

DevOps Learner | Linux Enthusiast | Automation Explorer

⭐ If you like this project

Give it a star ⭐ and feel free to fork and improve it.


---

# 🏗️ 2. Architecture Diagram


            ┌──────────────────────────┐
            │   Host Machine (Xubuntu) │
            │  Dell Latitude E7440     │
            └────────────┬─────────────┘
                         │
                 Ansible Playbook
                         │
 ┌───────────────────────┼───────────────────────┐
 │                       │                       │
 ▼                       ▼                       ▼

┌───────────┐ ┌────────────────┐ ┌─────────────────┐
│ Terraform │ │ VirtualBox │ │ AWS CLI │
│ Vagrant │ │ (VM Manager) │ │ Cloud Access │
└───────────┘ └───────┬────────┘ └─────────────────┘
│
▼
┌────────────────────────┐
│ DevOps Virtual Machines │
│ │
│ Docker │
│ Jenkins │
│ Grafana + Prometheus │
└────────────────────────┘
