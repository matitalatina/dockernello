Hello service
=========

A little example of a service that show an HTML page.

Role Variables
--------------

- `hello_docker_name`: the name of this docker container.
- `hello_domain`: the domain where you want to expose it.

Dependencies
------------

- (Ansible Role: Docker)[https://github.com/geerlingguy/ansible-role-docker]
- Docker Ingress Role: it's defined in this repo.

Example Playbook
----------------

```yaml
- hosts: all
  vars:
    hello_domain: hello.domain.com
  roles:
    - hello
```

License
-------

MIT
