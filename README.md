# ansible playbooks

all playbooks are called by this method from within the /etc/ansible folder
these methods are based on using pub+priv ssh key auth and not user+pass

this method will ask for input of the host name which you can use from your inventory/hosts file if you have set that up correctly
you can specify individual host or groups or all

# call playbook examples
0.     ansible-playbook playbooks/reboot.yml -K -i inventory/hosts
1.     ansible-playbook playbooks/createuser.yml -K -i inventory/hosts
2.     ansible-playbook playbooks/update_upgrade.yml -K -i inventory/hosts
3.     ansible-playbook playbooks/nanoinstall.yml -K -i inventory/hosts    
4.     ansible-playbook playbooks/githubsshkeychange.yml -K -i inventory/hosts
5.     ansible-playbook playbooks/dockerps.yml -K -i inventory/hosts
