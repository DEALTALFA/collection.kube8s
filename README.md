# Ansible Collection - cluster.k8
 ![](https://img.shields.io/badge/K8-s-red)    ![](https://img.shields.io/badge/Ansible-2.9.%2B-brightgreen)

Setup kubernetes cluster easily with kubeadm integrated With dynamic Inventory 

### Usage

To use specific role from the collection use in this format

```
- hosts: localhost
  remote_user: root
  roles:
	- dealtalfa.kubernetes.<role_name>
```
Tested on 
----------
AWS image :Amazon Linux 2 AMI

Dynamic Inventory
-----------------
To make the inventory dynamic for ec2 download 2 file `ec2.py` and `ec2.ini` from [here](https://github.com/ansible/ansible/tree/stable-2.9/contrib/inventory)
and follow the steps below

 * Make a new folder. let assume "myfolder"

 * download them into myfolder folder

   -  make them executable with command `chmod +x ec2.*`

 * type this in terminal to initalise environment variable that is used by dynamic inventory

   -  export AWS_ACCESS_kEY_ID=your_Access_Key

   -  export AWS_SECRET_ACCESS_KEY= your_secret_key

 * In ansible configuration file i.e. in path */ect/ansible/ansible.cfg*

    **Note:** If file don't exists make this file `ansible.cfg` in that path and write.
		
		[defaults]
		inventory= full_path/myfolder
		private_file=your_private_key
		remote_user=username
		[privilege_escalation]
		become=true
		become_method=sudo

for more information on _privilege_escalation_ [visit here](https://docs.ansible.com/ansible/latest/user_guide/become.html#become-directives) 			   
