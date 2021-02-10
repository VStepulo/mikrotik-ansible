# mikrotik-ansible

Gives you a possibility to distribute your ssh key on any Mikrotik device reached via a network. 

Pre-requirements:

0) You need to have Mikrotik device with SSH service enabled (IP - Services)
 
1) Edit and enter your IP and credentials in ./inventory/hosts file

3) Generated or installed id.rsa.pub key in your $HOME/.ssh/ dir.

4) Install required RouterOS community modules from Ansible galaxy:

	user@Ubuntu:~/mikrotik-ansible$ ansible-galaxy collection install -r requirements.yml
	
	
Run playbook by command:
	
	user@Ubuntu:~/mikrotik-ansible$ ansible-playbook play.yml
	
	
TODO:

Creating backups.
Update version.
