Ansible Firewall Role
=========

[![Build Status](https://travis-ci.org/rossedman/ansible-role-firewall.svg?branch=master)](https://travis-ci.org/rossedman/ansible-role-firewall)

A brief description of the role goes here.


Role Variables
--------------

```
firewall_open_ports: ["22", "80", "443"]
firewall_whitelist_ips:
  - "127.0.0.1/8"
firewall_bantime: "600"
firewall_maxretry: "3"
firewall_jail:
  ssh: true
  ssh_ddos: false
  apache: false
  php_url: false
  nginx_http: false

```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: servers
  roles:
     - { role: rossedman.Firewall, firewall_open_ports: ["22", "80", "443"] }
```
