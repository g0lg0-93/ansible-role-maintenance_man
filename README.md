# the Maintenance Man
Creating various roles to perform various tasks. 

Currently we have:
* Perform Update & Reboots (if required)
* Install unbound DNS

## Requirements
* Ansible

### Usage
Be sure to amend the `hosts:` portion of the playbook to the appropriate group of hosts. Otherwise, 
`hosts: all` will target all hosts. 
You can reference the appropriate playbook in the root directory.
`ansible-playbook <playbook file>`
_ Make sure your 'ansible.cfg' file knows your inventory, otherwise run the command like this: _
`ansible-playbook -i <inventory file> <playbook file>` 