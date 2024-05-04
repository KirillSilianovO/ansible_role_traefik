Ansible Traefik role
=========

Role for installation and configuration Traefik proxy

Requirements
------------

Docker installed and configured

Role Variables
--------------

`apps_root_dir` - Root directory for host application. `/opt/apps` by default.
`traefik_app_version` - Version of Traefik application
`traefik_dashboard_host_name` - Traefik dashboard DNS name

Dependencies
------------

- community.docker

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache
