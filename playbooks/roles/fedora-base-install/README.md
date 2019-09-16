# Fedora Base Install

Base install for Fedora workstations.

## Role Variables

| name                    | description                                            | type | default |
| ----------------------- | ------------------------------------------------------ | ---- | ------- |
| fedora_packages         | List of RPM packages to install                        | List | []      |
| fedora_python3_packages | List of Python 3 packages to install in user directory | List | []      |

## Example Playbook

```yaml
- hosts: workstations
  tasks:
  - import_role:
      name: fedora-base-install
    vars:
      fedora_packages:
        - vim
      fedora_python3_packages:
        - ipython
```

## License

MIT
