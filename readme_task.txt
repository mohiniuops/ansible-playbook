Steps to Launch ec2 machine with ansible playbook : 
1] Install Ansible :
pip3 install ansible
2] Make host file : 
lenovo@lenovo:~/Projects/playbooks$ cat /etc/ansible/hosts

localhost
lenovo@lenovo:~/Projects/playbooks$ 
3] Make a directory say playbook
mkdir playbook
cd playbook
4] Open AWS console : 
Go to IAM and make a user admin . Assign AmazonEC2FullAccess access to this user .
Download the accesskey csv file
Detailed steps in below youtube link : 
https://www.youtube.com/watch?v=gEX1HbM4KSM&t=304s
5] place task.yml in playbook folder and run below command : 
ansible-playbook task.yml
