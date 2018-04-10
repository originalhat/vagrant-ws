# vagrant-ws

reproducible development workstation

## boxes

>Instead of building a virtual machine from scratch, which would be a slow and tedious process, Vagrant uses a base image to quickly clone a virtual machine. These base images are known as "boxes" in Vagrant, and specifying the box to use for your Vagrant environment is always the first step after creating a new Vagrantfile.

```
vagrant box add hashicorp/precise64
```

## up and ssh

```
vagrant up
```

```
vagrant ssh
```

```
vagrant logout
```

## provisioning

```
vagrant reload --provision
```

cf. `bootstrap.sh`

## networking

```
vagrant reload
```

cf. `Vagrantfile`

## share

>Vagrant Share lets you share your Vagrant environment to anyone around the world with an Internet connection. It will give you a URL that will route directly to your Vagrant environment from any device in the world that is connected to the Internet.

```
vagrant plugin install vagrant-share
```

```
vagrant share --full
```

```
vagrant connect <host:port>
```

## teardown

1. suspend
2. halt
3. destroy

## providers

>While Vagrant ships out of the box with support for VirtualBox, Hyper-V, and Docker, Vagrant has the ability to manage other types of machines as well. This is done by using other providers with Vagrant.

```
vagrant up --provider=vmware_fusion
```

```
vagrant plugin install vagrant-aws
```

```
vagrant up --provider=aws
```

cf. https://github.com/mitchellh/vagrant-aws

