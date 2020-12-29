Docker Ingress role
=========

Install docker with nginx-proxy and nginx-proxy-companion to enable automated creation, renewal and use of Let's Encrypt certificates for proxied Docker containers.

Requirements
------------

Role Variables
--------------

- `admin_email`: your email required by Let's Encrypt.

Dependencies
------------

- [Ansible Role: Docker](https://github.com/geerlingguy/ansible-role-docker)
- `ansible-galaxy collection install community.general`

Example Playbook
----------------

```yaml
- hosts: all
  vars:
    admin_email: email@example.com
  roles:
    - hello
```

License
-------

MIT
