# ansible playbooks

all playbooks are called by this method from within the /etc/ansible folder
these methods are based on using pub+priv ssh key auth and not user+pass

this method will ask for input of the host name which you can use from your inventory/hosts file if you have set that up correctly
you can specify individual host or groups or all

# call playbook examples
.     ansible-playbook playbooks/reboot.yml -K -i inventory/hosts
     
.     ansible-playbook playbooks/createuser.yml -K -i inventory/hosts
     
.     ansible-playbook playbooks/update_upgrade.yml -K -i inventory/hosts
     
.     ansible-playbook playbooks/nanoinstall.yml -K -i inventory/hosts
     
.     ansible-playbook playbooks/githubsshkeychange.yml -K -i inventory/hosts
