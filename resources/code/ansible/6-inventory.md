## Ansible inventory

- Default localtion: /etc/ansible/host
- ansible -i my-host
- ansible.cfg

## Create inventory file

- touch $HOME/host
- edit host add the managed node IP
- ansible all -m command -a "pwd" -i host

## Create inventory groups

- edit $HOME/host
- create group
  [app]
  <app server ip address>

  [mail]
  <mail server ip address>

- ansible app -m command -a "pwd" -i host
