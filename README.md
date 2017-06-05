## Standalone GSTORE Deployment

- Requires Ansible 1.2 or newer
- Expects Ubuntu 14.04 hosts

Ensure you have ssh keypair auth setup with the host\hosts you wish to install on.

Edit group_vars/all with the dbnames and passwords of your choosing.

Follow either standalone or multi server setups below.




##Multi Server###
Edit the "hosts" inventory file by changing the IP addresses to the assicated addresses of the target servers.

Run the following:
ansible-playbook -i hosts vwp.yml



When the playbook run completes, log into the server and run "createapp" This will create the virtual env and finish the install.
Soon this will all be done in ansible.
