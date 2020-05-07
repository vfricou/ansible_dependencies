# README

Basic role to perform python3 installation on remote target in raw command

Use tags to select package manager

## Tags

| Tag | Description                                   |
|-----|-----------------------------------------------|
| apt | Perform installation with apt package manager |
| yum | Perform installation with yum package manager |

## Playbook

Here, a basic playbook to perform installation

```yaml
- name: install ansible dependencies on remote host
  hosts:
    - all
  strategy: free
  gather_facts: no
  roles:
    - ansible_dependencies
````
