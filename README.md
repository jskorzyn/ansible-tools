# Ansible Getting Started - Tools You Should Know

This demo introduces essential tools to enhance your Ansible automation journey. Learn how to efficiently manage, build, and run Ansible playbooks using modern tools and practices.

---

## Prerequisites

- Ansible installed
- Ansible-Navigator and Ansible-Builder installed or ansible-dev-tools
- Visual Studio Code (VS Code) installed
- Lightspeed access (Red Hat Ansible Lightspeed subscription or trial)
- Basic knowledge of Ansible playbooks and inventories

---

## Demo Steps

### Ansible-Navigator

Ansible-Navigator provides an enhanced CLI interface for Ansible users.

- **Run Playbook with Different Modes**

  ```bash
  # Traditional stdout output
  ansible-navigator run playbook.yml -i inventory -m stdout
  
  # Interactive mode with rich interface
  ansible-navigator run playbook.yml -i inventory
  ```

- **Replay a Previous Run**

View the results of a previous playbook execution:

```bash
ansible-navigator replay ansible-navigator-artifact-logs.json
```

- **View/Inspect Execution Environments (EEs)**

List available Execution Environments and inspect details:

```bash
ansible-navigator images
```

### Ansible-Builder

Ansible-Builder helps in creating custom Execution Environments (EEs) tailored for your automation tasks.

- **Build a Custom Execution Environment**

  ```bash
  cd /home/ansible/builder
  ansible-builder build -t custom-ee
  ```

### Visual Studio Code (VS Code)

Enhance your Ansible development workflow using VS Code.

- Install and showcase the **Ansible extension**.
- Explore **Ansible Development Tools** (linting, syntax checking, playbook validation).
- **Create EE templates** directly within VS Code.
- **Run playbooks** leveraging the newly built custom Execution Environment.

### Lightspeed with Ansible

Accelerate Ansible content creation using AI-powered assistance.

- **Task-by-Task Playbook Generation**
  - Get intelligent suggestions for each task in your playbook.
  
- **Full Playbook Generation**
  - Automatically generate complete playbooks from simple, natural language prompts.

## Expected Outcome

By the end of this demo, you will be familiar with:

- Running and managing playbooks efficiently using Ansible-Navigator.
- Replaying previous runs and inspecting Execution Environments.
- Building custom Execution Environments with Ansible-Builder.
- Developing playbooks faster and smarter with VS Code extensions.
- Leveraging AI to speed up playbook authoring with Lightspeed.

## Additional Resources

- [Ansible Documentation](https://docs.ansible.com/)
- [Ansible-Navigator GitHub](https://github.com/ansible/ansible-navigator)
- [Ansible-Builder GitHub](https://github.com/ansible/ansible-builder)
- [VS Code Ansible Extension](https://marketplace.visualstudio.com/items?itemName=redhat.ansible)
- [Ansible Lightspeed](https://www.redhat.com/en/technologies/management/ansible/ansible-lightspeed)
