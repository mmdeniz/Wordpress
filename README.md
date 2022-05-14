# Deploy Wordpress with Ansible on Ubuntu 20.04 LTS

### Steps to follow:

Lunch an EC2 instance on AWS with Ubuntu 20.04 LTS on it

Connect to the instance via ssh client

Create ssh keys, add them to the authorized keys, install ansible, clone the github repository and run the Ansible playbook with following the commands below:

### Create SSH keys and authorize them on the clint computer(s)`

ssh-keygen`

`cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys`

### Setup Ansible:

`sudo apt-get install -f`

`sudo apt-get install software-properties-common -y`

`sudo apt-add-repository ppa:ansible/ansible -y`

`sudo apt-get update`

`sudo apt-get install ansible -y`

### Clone the code repository

`cd ~`

`git clone https://github.com/mmdeniz/Wordpress.git`

### Run the Ansible Playbook

`cd Wordpress`

`ansible-playbook -i hosts install-wordpress.yml -vv`
