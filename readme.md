# K8s Ansible Cluster Deployment

Ansible playbook to deploy a Kubernetes cluster on Fedora Linux (or other RHEL-based distros)

## Instructions:

Create a key for ArgoCD to authenticate to your Git repo with

```bash
ssh-keygen -t ed25519 -f files/argocd_key -q -N ""
```

Grant the files/argocd_key.pub access to your git repo

Update the inventory.ini and vars.yml files with your details and run the playbook:

```bash
ansible-playbook -i inventory.ini deploy-cluster.yml
```