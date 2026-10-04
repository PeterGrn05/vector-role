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
| vector_config_dir       | Architecture of node system                                   |
| vector_data_dir         | Directory with logs to watch                                  |
| vector_config_path      | Directory with Ansible's generated Vector config              |
| vector_download_url     | Create or not test log file to watch                          |
| vector_install_dir      | Clickhouse port to connect via http                           |

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
