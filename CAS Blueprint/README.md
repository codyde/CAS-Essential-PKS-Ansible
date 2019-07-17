# CAS Requirements for Functionality

This blueprint was tested under the following conditions (which may or may not be best practice...)

## Conditions

* Ansible Open Source Integration bound to CAS using root credentials. No sudo checked.
* Ubuntu 18.04 as an OS for deployed resources
* SSH Key for Ansible server pushed to my vSphere template (ssh-copy-id is win)
* Hosts file for ansible stored at /etc/ansible/hosts
* The following directives applied in /etc/ansible/ansible.cfg

```ini
[defaults]
log_path=/var/log/ansible.log
display_skipped_hosts = false
hash_behaviour = merge
host_key_checking = False
inventory      = /etc/ansible/hosts
roles_path    = /root/playbooks/wardroom/ansible/roles
```
* When using Wardroom - ansible playbooks stored in /root/playbooks
* When using Wardroom - Wardcoom cloned into the /root/playbooks directory (navigate to directory, git clone https://github.com/codyde/wardroom for my forked repo)