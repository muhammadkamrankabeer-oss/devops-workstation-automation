Markdown# 🚀 DevOps Workstation Automation

![Banner](assets/banner.png)

Automated Linux DevOps environment setup using Ansible. This project transforms a fresh Xubuntu installation into a fully-equipped DevOps workstation in a single command.

---

## 📌 Overview
This project uses **Ansible** to provision a complete development environment on a local host. It is designed to demonstrate Infrastructure as Code (IaC) principles for local machine management.

**Designed for:**
*   DevOps Portfolio Showcase
*   Consistent Environment Reproducibility
*   Learning Infrastructure Automation

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
⚙️ Tech StackAutomation: AnsibleHost OS: Xubuntu (Linux)Virtualization: VirtualBox & VagrantInfrastructure: Terraform & AWS CLI📦 Installed ToolsCategoryToolsCoreGit, Curl, Wget, Vim, HtopNetworkingNet-tools, DNS utils, Traceroute, NmapDevOps/IaCTerraform, Vagrant, AWS CLI v2VirtualizationVirtualBoxProductivityVS Code, Brave Browser, OnlyOffice📂 Project StructureBashansible-setup/
├── assets/         # Images and banners
├── inventory       # Localhost connection details
├── setup.yml       # Main Ansible Playbook
└── README.md       # Project documentation
🚀 How to UseClone the repository:Bashgit clone [https://github.com/muhammadkamrankabeer-oss/devops-workstation-automation.git](https://github.com/muhammadkamrankabeer-oss/devops-workstation-automation.git)
cd devops-workstation-automation
Run the Playbook:Note: You will be prompted for your sudo password.Bashansible-playbook -i inventory setup.yml --ask-become-pass
🔄 CI/CD (GitHub Actions)This project uses a GitHub Actions pipeline to:Lint: Check YAML formatting.Validate: Ensure Ansible syntax is correct before deployment.👨‍💻 AuthorMuhammad Kamran KabeerDevOps Learner | Linux Enthusiast | Automation Explorer

LinkedIn https://www.linkedin.com/in/muhammad-kamran-kabeer-b64740a4/
| GitHub https://github.com/muhammadkamrankabeer-oss
