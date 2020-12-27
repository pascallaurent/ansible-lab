## Setup the Control Node (Ec2 Instance) - Red Hat

- Connect to the RedHat server
- sudo yum update
- sudo yum install python3 -y
- sudo alternatives --set python /usr/bin/python3
- python --version
- sudo yum -y install python3-pip
- sudo pip3 install awscli

## Setup the server hostname

- edit /etc/hostname
- change the host name
- Reconnect to see the change

## Create ansadmin user

- sudo useradd ansadmin
- sudo passwd ansadmin

## Add user to sudoer

- sudo visudo
- ansadmin ALL=(ALL) NOPASSWD: ALL

## Create SSH key

- su - ansadmin
- ssh-keygen
- Click the enter key all the way

## Enabled Password Basecd authentication

- vi /etc/ssh/ssh_config
- uncomment  PasswordAuthentication yes
- sudo service sshd restart
