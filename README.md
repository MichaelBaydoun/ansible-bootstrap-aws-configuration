# ansible-bootstrap-aws-configuration
Bootstrap my aws account

# Goal
With minimal manual work, configure a new aws account to the point ansible can run against it.  Then run bootstrap.yml (from a workstation external to aws) to provision an ansible server inside aws.

# Expection
The resulting aws ansible server will complete the configuration of the aws account and environment. 

# Instructions
- Create your aws account
- Create a group, create user and access key
- Download and save Key ID and Secret Access Key
- Add user to group
- [Install Ansible(https://docs.ansible.com/ansible/intro_installation.html)] on your Mac or linux workstation 
- sudo pip install boto
- Set AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, and AWS_REGION environment variables
    * Do this in a way that wont be recorded in yoru command history
- Run bootstrap playbook (ansible-playbook bootstrap.yml)

## Markdown
[Getting started guide (https://help.github.com/articles/basic-writing-and-formatting-syntax/)] to using markdown to format this README.md
