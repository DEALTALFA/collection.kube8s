# Ansible Collection - cluster.k8

Setup kubernetes cluster easily with kubeadm 

### Usage

To use specific role from the collection use in this format

```
- hosts: localhost
  remote_user: root
  roles:
	- dealtalfa.kubernetes.k8master
```