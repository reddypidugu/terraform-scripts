# Auto Provision of Jenkins Master on AWS

## Content

* Terraform Scripts for ec2 provsion and Jenkins install on it.
* Jenkins Install scripts
* README.md

Using these scripts you can automate the provision of Jenkins master on AWS EC2 instance.

* Before executing terraform apply command, login aws console and create a KeyPair and downlaod the 
publickey (*.pem). This key is will associated with ec2 instance and will be used to ssh to 
ec2 instance whenever it is needed.

* Once the key is generated and add the keyname. Please ensure the keypair must be created in the same region that you are 
going to provide ec2 instance.

Note: Finally dont forget to run "terraform destroy auto-approve" command to remove the resources you craeted 
via terraform, otherwise you will be charged by AWS for running resources.

