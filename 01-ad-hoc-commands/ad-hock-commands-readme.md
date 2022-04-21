# Ad-hoc commands examples

`ansible [pattern] -m [module] -a "[module options]“`
## Requirements
    - ansible module installed
    - hosts to test (or run this against localhost) 

## Ping module
`ansible -i inventory all -m ping`

## df-h command

`ansible -i inventory demo_server -a "df -h"`

## df-h command on localhost

`ansible 127.0.0.1 -a "df -h"`