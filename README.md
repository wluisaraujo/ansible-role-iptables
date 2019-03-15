[![Build Status](https://travis-ci.org/wluisaraujo/iac-ansible-iptables.svg?branch=master)](https://travis-ci.org/wluisaraujo/iac-ansible-iptables)
---
# IaC: with [Ansible](https://www.ansible.com) role to configure [Iptables](https://www.netfilter.org/)
------------

Description
------------

Configura iptables firewall Linux. Com suporte para IPv4
 
Requirements
------------

 * 


Role Variables
--------------

[defaults/main.yml](defaults/main.yml)

    firewall_state: started
    firewall_enabled_at_boot: true

Dependencies
------------

* None

Example Playbook
----------------
```yaml
---
- hosts: localhost
  vars_files:
    - vars/main.yml
  roles:
    - { role: iac-ansible-iptables }
...
```

License
-------

[GPLv3](https://www.gnu.org/licenses/gpl-3.0.pt-br.html)
