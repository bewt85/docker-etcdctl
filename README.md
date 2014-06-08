docker-etcdctl
==============

This is part of [mayfly](https://github.com/bewt85/mayfly) which demonstrates the 
concept of testing groups of versions of services in short lived virtual environments.

This container is used as the base of other containers which need to use etcd. It 
has etcd pre-installed and a script which makes it easier to pull common request 
parameteres from environment variables.

You can build your own versions of this container by setting the following environment variable 
to your docker index username (if you don't it uses mine) and running this bash script:

```
export DOCKER_ACCOUNT_NAME=<your_name>
sudo -E ./build.sh
```
