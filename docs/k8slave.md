# dealtalfa.kube8s.k8slave
 
 Configure the instances having tag `K8_slave` as Slave Node

## Role variables

None

## playbook example

    - hosts: localhost
      remote_user: root
      roles:
        - dealtalfa.kubernetes.k8slave
