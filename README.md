# 🧪 Zero-Budget GitOps Lab

A fully local, cost-free GitOps lab designed for learning, testing, and showcasing containerized applications on Kubernetes—powered by Ansible automation and a kind cluster. Perfect for DevOps experimentation without the cloud bill.

---

## 🚀 Features

- 🐳 **Containerized Application**: Build and deploy a local Python/Flask app via Docker.
- ☸️ **Kubernetes with kind**: Spin up a multi-node cluster using free-tier infrastructure.
- 🤖 **Ansible Automation**: Apply declarative manifests with clean, repeatable playbooks.
- 🔐 **No External Dependencies**: All services run locally. Ideal for air-gapped demos or secure labs.
- 🛠 **Professional Showcasing**: Easily share your project setup via GitHub with visual diagrams and clear workflows.

---

## 📁 Repo Structure

```bash
zero-budget-gitops-lab/
├── app/                        # Flask app + Dockerfile + requirements.txt
├── k8s/
│   └── base/                   # Kubernetes manifests (deployment + service)
├── ansible/
│   ├── inventory/
│   │   └── hosts.ini           # Local inventory
│   ├── playbooks/
│   │   └── deploy-app.yml      # Main Ansible playbook
│   └── roles/
│       └── deploy_app/
│           └── tasks/main.yml  # App deployment tasks
└── README.md
