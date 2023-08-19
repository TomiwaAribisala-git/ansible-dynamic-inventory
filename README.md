## Terraform and Ansible configuration for provisioning three AWS EC2 Instances, and starting docker containers on the instances via an ansible playbook dynamically using ansible plugins.

## Go to Terraform Config directory
```
cd terraform_config
```
## Terraform Commands
```
terraform init 
```

```
terraform validate 
```

```
terraform plan 
```

```
terraform apply
```


## Go to Ansible Config directory
```
cd ansible_config
```

## Adjust local docker compose file location at playbook 5th play
```
cat sala-docker-playbook.yml
```

## List the aws_ec2-plugin enabled instances
```
ansible-inventory -i inventory_aws_ec2.yml --graph
```

## Execute ansible playbook
```
ansible-playbook -i inventory_aws_ec2.yml sala-docker-playbook.yml
```