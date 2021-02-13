# Ansible Collection - cluster.k8
 ![](https://img.shields.io/badge/K8-s-red)    ![](https://img.shields.io/badge/Ansible-2.9.%2B-brightgreen)

Setup kubernetes cluster easily with kubeadm 

### Usage

To use specific role from the collection use in this format

```
- hosts: localhost
  remote_user: root
  roles:
	- dealtalfa.kubernetes.<role_name>
```
