Docker
=========

A role to install Docker and Docker Compose on a managed node

Requirements
------------

None

Notes
------------

Right now this role assumes the user is going to want to manage their docker containers through Ansible. This mean that the most recent Docker Compose supported right now is < 2.0.0. This role will not be updated for newer versions of docker-compose until the [community.docker.docker_compose](https://docs.ansible.com/ansible/latest/collections/community/docker/docker_compose_module.html) module is updated to support it.

Role Variables
--------------

- **docker_compose_version**: Placed for future compatibility.
  - Defaults to *latest when uncommented*

Dependencies
------------

No role dependencies.

Example Playbooks
----------------

```yaml
# Installs docker, and docker-compose 1.27 from Pip
    - role: 'irontooch.docker'
```

License
-------

GPL v3.0

Author Information
------------------

Author is IronTooch
