# Imagebuilder ansible role
Deploy imagebuilder with this ansible role

This has been tested to work with Ansible version 9.13 (ansible-core 2.16.3)
Ansible core 2.16 supports Python versions from 3.10 to 3.12

This role has dependencies which can be installed using
```bash
ansible-galaxy collection install -r requirements.yaml
```

An example playbook is included with this role under playbooks/mycloud.yaml
The example playbook is dependent on the following roles:
https://github.com/CSCfi/ansible-role-nrpe-plugins
https://github.com/CSCfi/ansible-role-nrpe

If you wish to not use NRPE then set the variable imagebuilder_manage_nrpe to false