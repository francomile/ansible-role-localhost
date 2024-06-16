# Ansible Localhost Role

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
