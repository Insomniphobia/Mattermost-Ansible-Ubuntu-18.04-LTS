1. Install ansible on your local machine and add the following to /etc/ansible/hosts:

[clients]
<ipaddress> or <fqdn> of remote server

2. If caddy2 is not installed run the caddy2 playbook first.

3. Create a user with sudo access on the remote server. Add your ssh key to ~/home/.ssh/authorized keys on the remote server. Use visudo, uncomment PubkeyAuthentication in /etc/ssh/sshd_config and change the value to yes.

4. run script using command ansible-playbook --ask-become-pass <playbook_name> 



