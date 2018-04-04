# ansible-role-letsencrypt
Tested on Ansible 2.4.2 and Ubuntu 16.04

## Playbook sample
This playbook installs certbot and issues cert from letsencrypt
```yaml
- hosts: registry
  become: yes
  roles:
    - role: letsencrypt
      domain: www.example.com
      email: admin@example.com
```
