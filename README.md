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
