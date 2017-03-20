# nginx-repo

- CNC: [![build status](https://source.cnc.sk/ansible/role-nginx-repo/badges/master/build.svg)](https://source.cnc.sk/ansible/role-nginx-repo/commits/master)
- GitHub: [![Build Status](https://travis-ci.org/hudecof/ansible_nginx_repo.svg?branch=master)](https://travis-ci.org/hudecof/ansible_nginx_repo)


Install official nginx repository, see **http://nginx.org/en/linux_packages.html**

## Role Variables

`nginx_repo_version` could be **[stable](http://nginx.org/en/linux_packages.html#stable)**(default) or **[mainline](http://nginx.org/en/linux_packages.html#mainline)**.

`nginx_repo_key` is the URL for the GPG public key usedto Sign the debian/ubuntu packages. Ypu do not need to change this value.

`nginx_repo_cache_dir` is the directorywhere is the `nginx_repo_key ` saved, defaults is **/tmp**. The `nginx_repo_key `is first downloadedand than imported. It wolrs like a local cache. In my playbooks I use value **{{playbook_dir}}/files/nginx**.

## Example Playbook

    - hosts: servers
      roles:
         - hudecof.nginx-repo

## License

BSD

## Author Information

Peter Hudec
CNC, a.s.
Slovakia
