# ansible_playbooks

all playbooks are called by this method from within the /etc/ansible folder
these methods are based on using pub+priv ssh key autha and not user+pass

this method will ask for host name which you can use from your inventory/hosts file if you have set that up correctly
you can specify individual host or groups or all

# example
1. ansible-playbook playbooks/reboot.yml -K -i inventory/hosts
2. ansible-playbook playbooks/createuser.yml -K -i inventory/hosts
