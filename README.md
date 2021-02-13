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

Dynamic Inventory
-----------------
To make the inventory dynamic inventory for ec2 download 2 file `ec2.py` and `ec2.ini` from [here](https://github.com/ansible/ansible/tree/stable-2.9/contrib/inventory)
and follow the steps below
 * Make a new folder. let assume myfile
 * download them into myfile folder
  - * make them executable with `chmod +x ec2.*`
 *  
   
