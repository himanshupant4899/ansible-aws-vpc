# ansible-aws-vpc
**The `vpc-setup.yml`present is used for following purpose:**
1. Create a new VPC
2. Create public and private subnets (3 each).
3. Configure networking (route-tables, IGW and NAT)

command for execution:
>ansible-playbook vpc-setup.yml

***

**The `bastion-instance.yml` is used for:**
1. Create a key-pair
2. Create security group
3. Launch bastion-instance

command for execution:
>ansible-playbook bastion-instance.yml
