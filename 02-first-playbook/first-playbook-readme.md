# Simple playbook to deploy file with specific content

## Requirements:
    - ansible module installed
    - hosts to test (or run this against localhost) 

## Modules:
- [Ansible playbook docs](https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html)
- [File](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/file_module.html)
- [Copy](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/copy_module.html)

## Usage:
`ansible-playbook -i [inventory] -l [subgroup,host] [playbook file]`

### All hosts from inventory
`ansible-playbook -i inventory create-file-with-content.yml`

### Selected Host
`ansible-playbook -i inventory -l [ip address, or hostaname, or group]create-file-with-content.yml`