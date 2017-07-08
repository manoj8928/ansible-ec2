# Spin up Instance /INstall nginx PHP and configure SSL on  AWS EC2 using Ansible

## Introduction

Naturally, you need [Ansible](http://ansibleworks.com) installed on your
host system before using this.

You will also need to export AWS_ACCESS_KEY and AWS_SECRET_KEY as environment
varibles before running the playbook. These are your AWS access values.

Then run ``ansible-playbook ec2.yaml -e 'keypair=FOO'`` where FOO is the name of your [AWS keypair](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html).


*NOTE*: The first part of the play, 'ec2.yaml' will create a new EC2 instance
**every time it is run**. This is the nature of the ec2 module.


