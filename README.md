# Fedora Workstation Playbooks

A collection of Ansible playbooks for setting up my Fedora workstation.

## Requirements

- Fedora 28 or later
- Ansible 2.5 or later

## Playbooks

| name                               | description                  |
| ---------------------------------- | ---------------------------- |
| [config.yml](playbooks/config.yml) | Configure Fedora workstation |

## Usage

1. Clone this Git repository and install the required roles.

```bash
git clone git@github.com:ghyde/ansible-playbooks-fedora-workstation.git
cd ansible-playbooks-fedora-workstation
ansible-galaxy install -r requirements.yml
```

2. Add your hosts to the provided [inventory](inventory) file.
3. Run the configuration playbook.

```bash
ansible-playbook -i inventory --ask-become-pass playbooks/config.yml
```

## License

[MIT](LICENSE)
