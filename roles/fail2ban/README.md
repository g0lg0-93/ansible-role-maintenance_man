Role Name
=========

Installing Fail2Ban.

Requirements
------------

Requires Ansible to perform the role. 
VM: Debian or Red Hat

Role Variables
--------------

defaults/main.yml - contains the default variables


Example Playbook
----------------
> fail2ban-playbook.yml

- hosts: {group of hosts or single host}
  become: yes
  gather_facts: yes
  vars_files:
    - vault/.vault_pitstop.yml {vault isn't required}
  roles:
    - fail2ban
  tags:
    - all, servers {I've set tags, you can remove tags if you have no use for them}
