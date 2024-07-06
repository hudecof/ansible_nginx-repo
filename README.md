# Repo: NGINX

Manage NGING official repositories.

# Requirements

For supported systems  see http://nginx.org/en/linux_packages.html. If yhour system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `nginx_repo_version`: the nginx version to install (__stable__ or __mainline__)
- `nginx_repo_state`: define presence of the repository

# Dependencies

There no external dependencies.

# Example Playbook

```
- hosts: servers
  roles:
     - hudecof.repo_nginx
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)