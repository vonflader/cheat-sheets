# Ansible
## Install Ansible on Ubuntu
1. Install PIP
```bash
sudo apt install python3-pip
```
2. Install Ansible
```bash
pip3 install ansible
```
3. Add execution path
```bash

```
4. Ansible example config: ansible.cfg
```bash
[defaults]
inventory=~/ansible/inventory/hosts
host_key_checking=False
```
5. Ansible config
```bash
#initialize default
ansible-config init
#view verbose
ansible-config view -v
```
7. Run ping on hosts from inventory (using user & pass)
```bash
ansible -i ./inventory/hosts local_ubuntu -m ping --user serveradmin --ask-pass
```
6. Run ping using default hosts from ansible.cfg (using user & pass)
```bash
ansible -i local_ubuntu -m ping --user serveradmin --ask-pass
```
7. Run playbook (using user & pass & become-pass)
```bash
ansible-playbook ./playbooks/playbook-name.yml --user serveradmin --ask-pass --ask-become-pass
```
