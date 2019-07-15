[![Ansible Galaxy](https://img.shields.io/badge/Ansible%20Galaxy-Firewall%20IPtables-blue.svg)](https://galaxy.ansible.com/wluisaraujo/iac-ansible-iptables) [![Build Status](https://travis-ci.org/wluisaraujo/ansible-role-iptables.svg?branch=master)](https://travis-ci.org/wluisaraujo/ansible-role-iptables)
# IaC: with [Ansible](https://www.ansible.com) role to configure [Iptables](https://www.netfilter.org/)
------------

Description
------------

Configura iptables firewall Linux. Com suporte para IPv4
 
Requirements
------------

 * 

Installation
------------

```console
vagrant@localhost:~$ ansible-galaxy install wluisaraujo.iptables
```


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
    - { role: iptables }
...
```

----------------
[![Licence](https://img.shields.io/badge/License-GPL%20v3-red.svg)](https://www.gnu.org/licenses/gpl-3.0.pt-br.html)
