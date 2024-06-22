# SLURM Setup

Ansible playbooks to set up SLURM

## Requirements

```shell
pipx install --include-deps ansible
```

## Usage

Add hostnames for SLURM controller and compute nodes in `staging.ini`.

Set account credentials to be used on the SLURM controller node in `roles/slurm/slurm_account_credentials`.

Run the playbook to set up SLURM on the controller node.

```shell
ansible-playbook -i staging.ini main_controller_roles.yml
```

Run the playbook to set up SLURM on the compute nodes.

```shell
ansible-playbook -i staging.ini main_compute_roles.yml
```
