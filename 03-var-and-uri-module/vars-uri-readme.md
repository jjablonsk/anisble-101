# Playbook example: URI custom vars and Ansible facts

## Requirements:
    - ansible module installed
    - hosts to test (or run this against localhost) 

## Modules:
- [Ansible Facts](https://docs.ansible.com/ansible/latest/user_guide/playbooks_vars_facts.html)
- [uri](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/uri_module.html)
- [Playbook variables](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html)

## Usage:
`ansible-playbook -i [inventory] -l [subgroup,host] [playbook file]`

### All hosts from inventory
`ansible-playbook -i inventory vars-uri-example.yml -e "MY_CUSTOM_VAR=thisismyvalue"`

### Selected Host
`ansible-playbook -i inventory -l [ip address, or hostaname, or group] vars-uri-example.yml -e "MY_CUSTOM_VAR=thisismyvalue"`