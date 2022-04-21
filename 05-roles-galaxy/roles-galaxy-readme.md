# Playbook example: Ansible Role and Ansible Galaxy

## Requirements:
    - ansible module installed
    - hosts to test (or run this against localhost)
    - installed role [ntp](https://galaxy.ansible.com/geerlingguy/ntp)

## Role:
- [ntp](https://galaxy.ansible.com/geerlingguy/ntp)

## Usage:
`ansible-galaxy install geerlingguy.ntp`

### All hosts from inventory
`ansible-playbook -i inventory configure-ntp.yml`

### Selected Host
`ansible-playbook -i inventory -l [ip address, or hostaname, or group] configure-ntp.yml`