Playbook: remove_spacewalk_centos7.yml
======================================

Tasks
-----
- Remove spacewalk specific files
- Remove spacewalk software and additions
- Remove spacewalk rpm key
- Remove enabled from /etc/yum/pluginconf.d/fastestmirror.conf
- Remove spacewalk unnecessary ssl files, remove /var/cache/yum directory
- Enable base,updates repos
- Run update-ca-trust

Usage
-----
- Run ansible playbook on CentOS VM
```bash
$ ansible-playbook -i <inventory> playbooks/remove_spacewalk_centos7/remove_spacewalk_centos7.yml -u ansible --ask-become-pass -l <hostname>
```
