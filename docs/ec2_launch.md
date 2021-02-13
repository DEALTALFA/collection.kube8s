
 # dealtalfa.kube8s.ec2_launch
 
 Role for launching Instance
 
- [ ]  **Master Node gets tag k8_master when launched**
- [ ]  **Slave Node gets tag k8_slave when launched**


## Role variables

* key
* AMI_imageinstance_type
* subnet
* aws_access
* aws_secret
* region 
* sg_group

Requirements
------------
boto module of python

Dependencies
------------
None

## Playbook example

    - hosts: localhost
      remote_user: root
      roles:
      - dealtalfa.kubernetes.ec2_launch
      
 License
-------

BSD

Author Information
------------------

[DEALTALFA@linkedIn](https://www.linkedin.com/in/deepak-yadav-588685127/)
