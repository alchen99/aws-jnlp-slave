# Docker JENKINS JNLP Slave with AWS CLI

This is a combination of https://github.com/jenkinsci/docker-slave and https://github.com/jenkinsci/docker-jnlp-slave with some added customization.

Jenkins JNLP Slave Container with AWS CLI and other things configured as follows:

* bash
* AWS CLI and aws-iam-authenticator
* kubectl
* curl
* jq

## Build

```
docker build -t alchen99/aws-jnlp-slave .
```

Automated build on Docker Hub

[![DockerHub Badge](http://dockeri.co/image/alchen99/aws-jnlp-slave)](https://hub.docker.com/r/alchen99/aws-jnlp-slave/)

## Usage

Configure:

```
export AWS_ACCESS_KEY_ID="<id>"
export AWS_SECRET_ACCESS_KEY="<key>"
export AWS_DEFAULT_REGION="<region>"
```

## References

* AWS CLI Docs: https://aws.amazon.com/documentation/cli/
* aws-iam-authenticator: https://github.com/kubernetes-sigs/aws-iam-authenticator
* kubectl: https://kubernetes.io/docs/reference/kubectl/overview/
* jq Manual: https://stedolan.github.io/jq/manual/
* jq Tutorial: https://stedolan.github.io/jq/tutorial/
