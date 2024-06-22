# SLURM Setup

Ansible playbooks to set up SLURM

## Requirements

```shell
pipx install --include-deps ansible
```

## Usage

Set account credentials to be used on the SLURM controller node in `roles/slurm/slurm_account_credentials`.

Then run the playbook to set up SLURM on the controller node.

```shell
ansible-playbook -i staging.ini main_controller_roles.yml
```
