Vector-role
=========

Роль Ansible для установки и конфигурации Vector.

Requirements
------------

- Ubuntu
- Ansible

Role Variables
--------------

| Vars                    | Description                                                   |
| ----------------------- | ------------------------------------------------------------- |
| vector_version          | Version of Vector to install                                  |
| vector_config_dir       | Configuration Directory for Vector                            |
| vector_data_dir         | Vector's Data directory                                       |
| vector_config_path      | Configuration Path for Vector                                 |
| vector_download_url     | Download URL for downloading Vector                           |
| vector_install_dir      | Installation directory                                        |

... и так далее

Example Playbook
----------------

```yaml
  - name: Install and configure Vector
  hosts: vector-01
  roles: vector-role
  become: true
  tags:
    - vector
```
License
-------

MIT

Author Information
------------------

Горин Пётр
