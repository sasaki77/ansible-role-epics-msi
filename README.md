# Ansible Role: EPICS Gateway

Installs EPICS msi on RHEL/CentOS.

## Requirements

- ansible >= 2.3

## Role Variables
Refer to `defaults/main.yml` in detail.
```
msi_extension: 
  url: "https://www.aps.anl.gov/epics/download/extensions/msi1-7.tar.gz"
  unarchived_name: "msi1-7"
  release: false
```

## Dependencies

- [ansible-role-epics-base](https://github.com/sasaki77/ansible-role-epics-base)

## Example Playbook
```
- hosts: epics-base
  roles:
    - role: ansible-role-epics-base
    - role: ansible-role-epics-msi
```

## License

None.

## Author Information

This role was created by Shinya Sasaki.
