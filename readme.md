# Ansible Kubernetes Cluster Deployment

Ansible playbook to deploy a Kubernetes cluster on RHEL-like distros (tested with Fedora 38)

Update the inventory and variable files with your details and run:

```bash
ansible-playbook -i inventory.ini deploy-cluster.yml
```