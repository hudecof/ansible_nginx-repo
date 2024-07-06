# Repo: NGINX

Manage NGINX official repositories.

# Requirements

For supported systems  see http://nginx.org/en/linux_packages.html. If your system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `nginx_repo_version_stable`: if __true__, the stable repository will be added
- `nginx_repo_version_mainline`: if __true__, the mainline repository will be added
- `nginx_repo_state`: define presence of the repository, if __false__, the rpeository will be removed

# Dependencies

There no external dependencies.

# Example Playbook

```
- hosts: servers
  roles:
     - hudecof.nginx_repo
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)