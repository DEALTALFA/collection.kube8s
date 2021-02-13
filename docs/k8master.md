# dealtalfa.kube8s.k8master
 
 Configure the instances having tag `K8_master` as Master Node

## Role variables

None

## playbook example

    - hosts: localhost
      remote_user: root
      roles:
        - dealtalfa.kubernetes.k8master
