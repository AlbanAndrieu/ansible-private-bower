## alban.andrieu.private-bower

[![Travis CI](http://img.shields.io/travis/AlbanAndrieu/ansible-private-bower.svg?style=flat)](http://travis-ci.org/AlbanAndrieu/ansible-private-bower) [![Branch](http://img.shields.io/github/tag/AlbanAndrieu/ansible-private-bower.svg?style=flat-square)](https://github.com/AlbanAndrieu/ansible-private-bower/tree/master) [![Donate](https://img.shields.io/gratipay/AlbanAndrieu.svg?style=flat)](https://www.gratipay.com/AlbanAndrieu)  [![Ansible Galaxy](http://img.shields.io/badge/galaxy-alban.andrieu.privatebower-blue.svg?style=flat)](https://galaxy.ansible.com/list#/roles/2852) [![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)

Ensures that [private-bower](https://www.npmjs.com/package/private-bower) is properly installed and configured.

### Installation

This role requires at least Ansible `v1.6.3`. 

To install it, run:

    ansible-galaxy install alban.andrieu.private-bower

### Role dependencies

- `nodejs`

### Role variables

List of default variables available in the inventory:

```yaml
        private_bower_enabled: yes                       # Enable module
    
    private_bower_version: "0.6.5"
    private_bower_base_dir: "/usr/local/lib/node_modules/private-bower"
    
    private_bower_backup_enabled: false                       # Enable backup
    private_bower_backup_host: "backup-server"
    private_bower_backup_user: "bower"
    private_bower_backup_dir: "backup"
    private_bower_backup: "{{ private_bower_backup_user }}@{{ private_bower_backup_host }}::{{ private_bower_backup_dir }}"
```


### Detailed usage guide

Describe how to use in more detail...


### Authors and license

`alban.andrieu.private-bower` role was written by:
- [Alban Andrieu](fr.linkedin.com/in/nabla/) | [e-mail](mailto:alban.andrieu@free.fr) | [Twitter](https://twitter.com/AlbanAndrieu) | [GitHub](https://github.com/AlbanAndrieu)
- License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/AlbanAndrieu/ansible-private-bower/issues)!

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
