# ansible_k8s

[Installation Guide]

Install ansible on your machine/work station
1. RedHat OS Distributions
  - sudo yum update -y
  - sudo yum install epel-release -y
  - sudo yum install ansible -y

2. Debian OS Distributions
  - sudo apt-add-repository ppa:ansible/ansible
  - sudo apt update -y
  - sudo apt install ansible -y

[Configuration]

1. Setup inventory : Add the hosts to the /etc/ansible/hosts
2. Authentication using SSH key : 
   - "ssh-keygen" #Run this command at your workstation machine in ~/.ssh public key file will be generated id_rsa.pub
   - Copy the content of the file id_rsa.pub and paste it to all remote machines/nodes in ~/.ssh/authorized_keys file (if file doesn't exist on nodes then create the file)
   OR
   - ssh-copy-id user@ip #Run this command to copy key 
