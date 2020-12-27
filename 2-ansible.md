## Installing Ansible

- su - ansadmin
- pip3 install ansible --user

## Make sure ansible is installed

- ansible --version

# Ansible configuration file

- sudo mkdir /etc/ansible
- cd /etc/ansible
- sudo vi ansible.cfg
- copy the content of <https://raw.githubusercontent.com/ansible/ansible/devel/examples/ansible.cfg> to ansible.cfg
- sudo touch hosts
