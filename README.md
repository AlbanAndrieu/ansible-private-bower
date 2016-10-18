## [![Nabla](https://debops.org/images/debops-small.png)](https://github.com/AlbanAndrieu) alban_andrieu_private_bower

<!-- This file was generated by Ansigenome. Do not edit this file directly but
     instead have a look at the files in the ./meta/ directory. -->

[![Travis CI](https://img.shields.io/travis/AlbanAndrieu/ansible-private-bower.svg?style=flat)](https://travis-ci.org/AlbanAndrieu/ansible-private-bower)
[![Branch](http://img.shields.io/github/tag/AlbanAndrieu/ansible-private-bower.svg?style=flat-square)](https://github.com/AlbanAndrieu/ansible-private-bower/tree/master)
[![Donate](https://img.shields.io/gratipay/AlbanAndrieu.svg?style=flat)](https://www.gratipay.com/AlbanAndrieu)
[![test-suite](https://img.shields.io/badge/test--suite-ansible--alban__andrieu__private__bower-blue.svg?style=flat)](https://github.com/AlbanAndrieu/test-suite/tree/master/ansible-alban_andrieu_private_bower/)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-alban.andrieu.private--bower-660198.svg?style=flat)](https://galaxy.ansible.com/detail#/role/2852)
[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)
[![Gittip](http://img.shields.io/gittip/alban.andrieu.svg)](https://www.gittip.com/alban.andrieu/)
[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=AlbanAndrieu&url=https://github.com/alban.andrieu/ansible-phpvirtualbox&title=Ansible Role: PhpVirtualbox&language=&tags=github&category=software)

Ensures that [private-bower](https://www.npmjs.com/package/private-bower) is properly installed and configured.


### Role dependencies

- `nodejs`
### Installation

This role requires at least Ansible `v2.1.1`. To install it, run:

Using `ansible-galaxy`:
```shell
$ ansible-galaxy install alban.andrieu.private-bower
```

Using `arm` ([Ansible Role Manager](https://github.com/mirskytech/ansible-role-manager/)):
```shell
$ arm install alban.andrieu.private-bower
```

Using `git`:
```shell
$ git clone https://github.com/alban.andrieu/ansible-eclipse.git
```

### Documentation

More information about `alban.andrieu.private-bower` can be found in the
[official alban.andrieu.private-bower documentation](https://docs.debops.org/en/latest/ansible/roles/ansible-private-bower/docs/).


### Role variables

List of default variables available in the inventory:

```YAML
private_bower_enabled: yes                       # Enable module

private_bower_version: "1.0.7"
private_bower_base_dir: "/usr/local/lib/node_modules/private-bower"
private_bower_conf: "bower.conf.json"

private_bower_repository_cache_cache_private: "false"
private_bower_repository_cache_git_enabled: "true"
private_bower_authentication_enabled: "false"
private_bower_authentication_key: "password"

private_bower_backup_enabled: false                       # Enable backup
private_bower_backup_host: "backup-server"
private_bower_backup_user: "bower"
private_bower_backup_dir: "backup"
private_bower_backup: "{{ private_bower_backup_user }}@{{ private_bower_backup_host }}::{{ private_bower_backup_dir }}"

# Package states: present or installed or latest
private_bower_pkg_state: present

shell_git_ssl: "false"
```


### Detailed usage guide

Describe how to use in more detail...


### Authors and license

`alban_andrieu_private_bower` role was written by:

- [Alban Andrieu](fr.linkedin.com/in/nabla/) | [e-mail](mailto:alban.andrieu@free.fr) | [Twitter](https://twitter.com/AlbanAndrieu) | [GitHub](https://github.com/AlbanAndrieu)

- License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

Copyright (c) 2016 [Alban Andrieu](https://alban-andrieu.com/)

### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/AlbanAndrieu/ansible-private-bower/issues)!

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests and examples for any new or changed functionality.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

***

This role is part of the [Nabla](https://github.com/AlbanAndrieu) project.
README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
