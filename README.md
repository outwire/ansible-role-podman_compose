Ansible Role Podman Compose
=========

![ci](https://github.com/outwire/ansible-role-podman_compose/workflows/ci/badge.svg)
![quality](https://img.shields.io/ansible/quality/52935)
![license](https://img.shields.io/github/license/outwire/ansible-role-podman_compose)

Install podman-compose

Role Variables
--------------

    podman_compose_install_method: "git"

Source of podman-compose, either from `git` or `pip`

    podman_compose_version_git: "devel"

If `podman_compose_install_method` is set to `git`, the podman-compose version to be installed from git.

    podman_compose_version_pip: ""

If `podman_compose_install_method` is set to `pip`, the podman-compose version to be installed from pip. If not set, the latest version will be installed.

    podman_compose_path_git: /usr/local/bin/podman-compose

If `podman_compose_install_method` is set to `git`, the destination of podman-compose.


Dependencies
------------

None

Example Playbook
----------------

Install development version from git:

    - hosts: servers
      roles:
         - role: outwire.podman_compose

License
-------

MIT
