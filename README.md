# Wordpress

ssh-keygen

cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys

Setup Ansible:

sudo apt-get install -f

sudo apt-get install software-properties-common -y

sudo apt-add-repository ppa:ansible/ansible -y

sudo apt-get update

sudo apt-get install ansible -y

cd ~

git clone https://github.com/mmdeniz/Wordpress.git

cd Wordpress

ansible-playbook -i hosts install-wordpress.yml -vv
