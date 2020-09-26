Support for my Packer training on Udemy

```Learn DevOps: Infrastructure Automation With Terraform``` by ```Edward Viaene```

## Create an AMI containing Ansible
docker run \
-v `pwd`:/tmp/wd \
-w /tmp/wd \
-v /Users/fdebuire/.ssh:/tmp/.ssh \
hashicorp/packer:light \
build ansible-ami.json

`pwd` is mounted so the scripts folder can be used in the provisioners section.
Same for the `.ssh` folder.