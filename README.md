# docker-aws-cli

A convenient image used to run aws cli commands

## Examples

Getting started :

```
$ docker pull vidarl/docker-aws-cli
$ docker run --rm -ti -v ${HOME}/.aws/credentials:/root/.aws/credentials -v ${HOME}/.aws/config:/root/.aws/config vidarl/docker-aws-cli aws ec2 describe-instances
```


The image is quite convenient to use if you make an alias:


```
$ alias aws="docker run --rm -ti -v ${HOME}/.aws/credentials:/root/.aws/credentials -v ${HOME}/.aws/config:/root/.aws/config vidarl/docker-aws-cli aws"

$ # Now you may use this alias to run the CLI
$ aws ec2 descrive-instances

```
