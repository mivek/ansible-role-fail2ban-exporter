Fail2ban Exporter
=========

This role installs a Prometheus exporter collecting metrics on fail2ban.

https://github.com/mivek/fail2ban_exporter

Requirements
------------

None.

Role Variables
--------------

| Name                      | Description                            | Default value |
|---------------------------|----------------------------------------|---------------|
| fail2ban_exporter_version | The version of the exporter to install | 0.0.2         |
| fail2ban_exporter_port    | The port to expose the metrics on      | 9921          |


Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: all
  tasks:
    - name: "Include mivek.fail2ban_exporter"
      include_role:
        name: "mivek.fail2ban_exporter"
```
License
-------

BSD

