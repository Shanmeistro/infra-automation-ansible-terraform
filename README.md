# Infrastructure Automation with Terraform and Ansible

## Overview

This project demonstrates automated infrastructure provisioning and configuration on **AWS** and **Azure** using **Terraform** and **Ansible**. It provides a template for setting up both cloud-native and hybrid cloud environments.

## Features

- **Terraform**: Automates provisioning of infrastructure, including VMs, networks, and storage.
- **Ansible**: Configures provisioned resources, such as installing web servers and applying security hardening.
- **CI/CD Pipeline**: Automates the deployment and configuration process.
- Modular design for use with both AWS and Azure.

## Requirements

- Terraform (`>= 1.x`)
- Ansible (`>= 2.x`)
- Cloud provider credentials (AWS or Azure)

## Getting Started

### Clone the Repository

```
git clone https://github.com/your-username/infra-automation-ansible-terraform.git
cd infra-automation-ansible-terraform
```

### Set Up Terraform

1.  Navigate to the `terraform/aws/` or `terraform/azure/` directory.
2.  Configure the `variables.tf` file.
3.  Run the following commands:

```
terraform init
terraform apply
```

### Run Ansible Playbooks

1.  Navigate to the `ansible/` directory.
2.  Configure the inventory files in `inventories/aws/` or `inventories/azure/`.
3.  Execute playbooks:

```
ansible-playbook playbooks/webserver.yml -i inventories/aws/hosts
```

### **Folder Structure**

    infra-automation-ansible-terraform/
    ├── terraform/         # Infrastructure provisioning
    │   ├── aws/           # AWS Terraform scripts
    │   ├── azure/         # Azure Terraform scripts
    ├── ansible/           # Server configuration
    │   ├── playbooks/     # Ansible playbooks
    │   ├── inventories/   # Inventory files for environments
    ├── ci-cd/             # CI/CD automation
    │   ├── .github/       # GitHub Actions workflows
    ├── README.md          # Documentation
    ├── LICENSE            # License information

## Contributing

We welcome contributions! Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

