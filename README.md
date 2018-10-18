# nginx-lb
Launch Ec2 and configure Nginx LB with Ansible

~/.boto - aws Credentials or export 

- Using launch-ec2.yml can create ec2 instances on AWS 

$ ansible-playbook launch-ec2.yml	 

- number of instances can controlled by variable " count: " 


$ ansible-playbook site.yml 

- LB instanaces 
     act like jumphost for accessing private instances. 

- Has two roles 
   first to install nginx LoadBalancer 
   second to install nginx webserver behind LB with no IG 
   
