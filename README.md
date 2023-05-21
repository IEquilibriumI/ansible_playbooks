# ansible_playbooks

all playbooks are called by thos method from within the /etc/ansible folder
these methods are based on using pub+priv ssh key autha and not user+pass

# example
ansible-playbook playbooks/reboot.yml -K -i inventory/hosts
