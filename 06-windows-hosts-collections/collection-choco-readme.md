# Playbook example: Ansible Collection and Choco

## Requirements:
    - ansible module installed
    - hosts to test (or run this against localhost)
    - installed collection [windows](https://galaxy.ansible.com/ansible/windows)

## Role:
- [win_reboot](https://docs.ansible.com/ansible/latest/collections/ansible/windows/win_reboot_module.html)
- [win_chocolatey](https://docs.ansible.com/ansible/latest/collections/chocolatey/chocolatey/win_chocolatey_module.html)
- [win_wait_for](https://docs.ansible.com/ansible/latest/collections/ansible/windows/win_wait_for_module.html)

## Usage:
`ansible-galaxy collection install ansible.windows`

### All hosts from inventory
`ansible-playbook -i inventory collection-choco-windows.yml`

### Selected Host
`ansible-playbook -i inventory -l [ip address, or hostaname, or group] collection-choco-readme.yml`