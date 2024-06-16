# Ansible Localhost Role

[![Lint Ansible roles](https://github.com/francomile/ansible-role-localhost/actions/workflows/ansible_lint.yml/badge.svg)](https://github.com/francomile/ansible-role-localhost/actions/workflows/ansible_lint.yml)

[![Release role to Ansible Galaxy](https://github.com/francomile/ansible-role-localhost/actions/workflows/push_to_galaxy.yml/badge.svg)](https://github.com/francomile/ansible-role-localhost/actions/workflows/push_to_galaxy.yml)

## Actions of the Role

* Create a loopback alias interface (100.64.64.64 by default).

## Common Usage

```yaml
roles:
  - {
    role: localhost,
    localhost_alias_ip: "100.64.64.64",
    tags: ["netplan"]
  }
```

## Run the playbook

```shell
ansible-playbook -i inventory playbook.yaml -t "localhost"
```
