# Playbook example: include tasks, async/poll, get_url

## Requirements:
    - ansible module installed
    - hosts to test (or run this against localhost) 

## Modules:
- [get_url](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/get_url_module.html)
- [Asynchronous actions and polling](https://docs.ansible.com/ansible/latest/user_guide/playbooks_async.html)
- [include_task](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/include_tasks_module.html)
- [import_task](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/import_tasks_module.html)

## Usage:
`ansible-playbook -i [inventory] -l [subgroup,host] [playbook file]`

### All hosts from inventory
`ansible-playbook -i inventory import-async-example.yml`

### Selected Host
`ansible-playbook -i inventory -l [ip address, or hostaname, or group] import-async-example.yml`