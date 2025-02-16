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
`traefik_acme_email` - Email for Let's Encrypt

Dependencies
------------

- community.docker

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
- hosts: servers
  roles:
    - role: traefik
      vars:
          apps_root_dir: '/opt/apps'
          traefik_app_version: 3.3.3
          traefik_dashboard_host_name: 'traefik.example.com'
          traefik_acme_email: 'ksilyanov@proton.me'
      tags:
        - hs_traefik
```

License
------
    -

Apache
