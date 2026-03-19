
---

# 🚀 Ansible for DevOps

A practical, project-based guide to mastering Ansible for DevOps—covering automation, configuration management, and real-world infrastructure use cases.

---

## 📌 About This Repository

This repository is designed to help you learn **Ansible from beginner to advanced level** with hands-on examples and real-world DevOps scenarios.

Whether you're starting out or already working in DevOps, this repo will help you:

* Automate infrastructure and deployments
* Manage configuration at scale
* Write clean, reusable Ansible playbooks
* Apply production-ready automation patterns

---

## 🧭 Learning Path

```
00-basics            → Introduction & setup  
01-inventory         → Static & dynamic inventory  
02-adhoc-commands    → Quick automation tasks  
03-playbooks         → Writing playbooks  
04-variables         → Managing variables  
05-handlers          → Event-driven automation  
06-roles             → Reusable role structure  
07-templates         → Jinja2 templating  
08-security          → Vault & secrets  
09-cloud             → Cloud integrations  
10-projects          → Real-world use cases  
```

---

## 🛠️ Prerequisites

* Basic Linux knowledge
* SSH access to servers
* Python installed
* Ansible installed

### Install Ansible

```bash
pip install ansible
```

---

## 📂 Repository Structure

```
ansible-for-devops/
│
├── inventory/
├── playbooks/
├── roles/
├── projects/
│
├── 00-basics/
├── 01-inventory/
├── ...
├── 10-projects/
│
├── ansible.cfg
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/eknatha/ansible-for-devops.git
cd ansible-for-devops
```

### 2. Create an inventory file

```ini
[web]
your-server-ip
```

### 3. Run your first playbook

```bash
ansible-playbook -i inventory playbooks/setup.yml
```

---

## 💡 Example Playbook

```yaml
- name: Install Nginx
  hosts: web
  become: yes

  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present
```

---

## 📦 Projects Included

* ✅ Setup Nginx server
* ✅ Deploy a Node.js application
* ✅ Server hardening
* ✅ User & SSH management
* ✅ Monitoring setup
* ✅ Multi-tier infrastructure automation

---

## 🔐 Security

* Ansible Vault for secrets management
* Secure SSH practices
* Least privilege principles

---

## 🧠 What You’ll Learn

* Infrastructure as Code (IaC) with Ansible
* Idempotent automation
* Role-based architecture
* Production-ready playbooks
* CI/CD integration

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a new branch
3. Submit a pull request

---

## ⭐ Support

If you find this repo helpful, give it a ⭐ on GitHub!

---

## 👨‍💻 Author

**Eknatha**
🔗 [https://github.com/eknatha](https://github.com/eknatha)

---

## 🏁 Related Repositories

* linux-100-devops-challenge
* linux-for-devops
* terraform-playbook
* terraform-production-patterns
* kubernetes-production-runbooks

---

Happy Automating with Ansible ⚡
