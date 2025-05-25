# ansible-spotify
[![Static Badge](https://img.shields.io/badge/Ansible_galaxy-Download-blue)](https://galaxy.ansible.com/ui/repo/published/compscidr/spotify/)
[![ansible lint](https://github.com/compscidr/ansible-spotify/actions/workflows/check.yml/badge.svg)](https://github.com/compscidr/ansible-spotify/actions/workflows/check.yml)
[![ansible lint rules](https://img.shields.io/badge/Ansible--lint-rules%20table-blue.svg)](https://ansible.readthedocs.io/projects/lint/rules/)

Ansible collection to install spotify

## Usage:
Add the collection to your meta/requirements.yml:
```
collections:
  - name: compscidr.spotify
    version: "<insert version here>"
```

Use the role(s) in a playbook:
```
- name: Install spotify
  hosts: all
  roles:
    - spotify
```

## Testing:
Using molecule:
```
python -m venv venv
. venv/bin/activate
pip install molecule molecule-docker passlib
molecule test
```