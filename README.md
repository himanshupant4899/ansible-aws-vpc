# Ansible for AWS
The `vpc-setup.yml` playbook is responsible for creating a new AWS VPC consisting of 3 public subnets and 3 private subnets configured.

The bastion-host is created and configured through the `bastion-instance.yml` playbook.

Both the above mentioned playbook have been imported to the `site.yml` playbook as follows:

```YAML
---
- import_playbook: vpc-setup.yml
- import_playbook: bastion-instance.yml
```
***
**Command to execute the final playbook:**
>$ ansible-playbook site.yml
