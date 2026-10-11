# Ansible Playbook Collection ⚙️

A hands-on collection of Ansible playbooks created to practice Linux administration, configuration management, and infrastructure automation.

The repository covers common administrative tasks and provides a foundation for building repeatable, maintainable automation workflows.

## 🎯 Objectives

- Automate common Linux administration tasks.
- Practice Ansible playbook structure and YAML syntax.
- Manage packages, services, users, and groups.
- Work with variables, templates, and registration of task results.
- Develop reusable automation workflows for infrastructure operations.

## 🛠️ Playbook Catalog

| Playbook | Focus |
|---|---|
| `package_install.yml` | Package installation |
| `precheck.yml` | Pre-execution checks |
| `register_out.yml` | Capturing task results using registered variables |
| `service_manager.yml` | Service management |
| `template.yml` | Template-based configuration |
| `test.yml` | Ansible practice and testing |
| `usergroup.yml` | User and group management |
| `var.yml` | Variables in playbooks |

*Descriptions are based on filenames and should be verified against each playbook's implementation.*

## ⚙️ Prerequisites

- Ansible installed on the control node
- SSH connectivity to the target Linux hosts
- A valid inventory file
- Appropriate privileges on managed hosts
- Python and required dependencies on managed nodes, as applicable

## 🚀 Getting Started

Check the installed Ansible version:

```bash
ansible --version
```

Validate YAML/playbook syntax:

```bash
ansible-playbook -i inventory.ini package_install.yml --syntax-check
```

List the tasks in a playbook:

```bash
ansible-playbook -i inventory.ini service_manager.yml --list-tasks
```

Run a playbook after reviewing its tasks and target hosts:

```bash
ansible-playbook -i inventory.ini precheck.yml --check
```

Note: Check mode is a simulation and may not fully predict every task's behavior. Review the playbook before executing it against any real infrastructure.

## 🔐 Security Practices

- Never commit passwords, private keys, tokens, or production credentials.
- Use Ansible Vault or an approved secrets manager for sensitive variables.
- Keep inventories free of confidential hostnames and internal infrastructure details.
- Test playbooks against disposable lab hosts before production use.
- Review changes and privilege escalation requirements before execution.

## 📚 Skills Demonstrated

Ansible · YAML · Linux Administration · Configuration Management · Variables · Jinja2 Templates · Service Management · Package Management · Infrastructure Automation

## 👨‍💻 Author

**Anurag Utkarsh**

[GitHub Profile](https://github.com/AnuragUtkarsh)
