<h1 align="center">🚀 DevOps Workstation Automation</h1>

<p align="center">
Automated Linux DevOps environment setup using Ansible (Terraform • VirtualBox • AWS CLI)
</p>

<p align="center">
<img src="https://img.shields.io/badge/Ansible-Automation-red?style=for-the-badge" alt="Ansible">
<img src="https://img.shields.io/badge/Terraform-IaC-purple?style=for-the-badge" alt="Terraform">
<img src="https://img.shields.io/badge/VirtualBox-VM-blue?style=for-the-badge" alt="VirtualBox">
<img src="https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge" alt="AWS CLI">
<img src="https://img.shields.io/badge/Linux-Ubuntu-yellow?style=for-the-badge" alt="Linux">
<img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Status">
<img src="https://github.com/muhammadkamrankabeer-oss/devops-workstation-automation/actions/workflows/ci.yml/badge.svg" alt="CI">
</p>

---

## 📌 Overview
This project uses **Ansible** to provision a complete development environment on a local host. It is designed to demonstrate Infrastructure as Code (IaC) principles for local machine management.

**Designed for:**
*   DevOps Portfolio Showcase
*   Consistent Environment Reproducibility
*   Learning Infrastructure Automation

---

## 🏗️ Architecture
The following diagram illustrates how the automation layers are structured on the host machine:

```mermaid
graph TD
    A[Dell E7440 Host - Xubuntu] --> B[Ansible Playbook]
    B --> C[System Utilities]
    B --> D[DevOps Toolchain]
    B --> E[Virtualization Layer]
    
    subgraph "Installed Tools"
    C --> C1[Git / Vim / Htop]
    C --> C2[Net-tools / Nmap]
    D --> D1[Terraform]
    D --> D2[AWS CLI v2]
    D --> D3[VS Code]
    E --> E1[VirtualBox]
    E --> E2[Vagrant]
    end
    
    subgraph "Planned Labs"
    E1 --> F[Docker VM]
    E1 --> G[Jenkins CI/CD]
    E1 --> H[Monitoring Stack]
    end
⚙️ Tech StackAutomation Engine: AnsibleHost System: Xubuntu (Linux)Virtualization: VirtualBox & VagrantCloud Tools: Terraform & AWS CLI📦 Installed ToolsCategoryToolsCore SystemsGit, Curl, Wget, Vim, HtopNetworkingNet-tools, DNS utils, Traceroute, NmapDevOps & IaCTerraform, Vagrant, AWS CLI v2VirtualizationVirtualBoxProductivityVS Code, Brave Browser, OnlyOffice📂 Project StructureBashansible-setup/
├── assets/         # Images and banners
├── inventory       # Localhost connection details
├── setup.yml       # Main Ansible Playbook
└── README.md       # Project documentation
🚀 How to Use1. Clone the repositoryBashgit clone [https://github.com/muhammadkamrankabeer-oss/devops-workstation-automation.git](https://github.com/muhammadkamrankabeer-oss/devops-workstation-automation.git)
cd devops-workstation-automation
2. Run the PlaybookNote: You will be prompted for your sudo password to install packages.Bashansible-playbook -i inventory setup.yml --ask-become-pass
🔄 CI/CD (GitHub Actions)This project uses a GitHub Actions pipeline to:Lint: Check YAML formatting.Validate: Ensure Ansible syntax is correct before deployment.👨‍💻 AuthorMuhammad Kamran KabeerDevOps Learner | Linux Enthusiast | Automation ExplorerLinkedIn | GitHub
