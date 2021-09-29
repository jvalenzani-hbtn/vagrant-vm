# Ubuntu - Docker 

Vagrant file with Ubuntu focal64 (20.04) image and docker / docker-compose provisioner

For testing and development.

## Instructions

0. You'll need vagrant and VirtualBox installed on the host computer.

If you cloned the repo, jump to step 4.

1. Create a folder for the project

2. Copy VagrantFile to the new created folder

3. On the project folder create a new folder called `data` that will be mounted to the vm in `/vagrant_data`.
This is in case you need to share files easily between the VM and the host machine.

4. Install required vagrant plugins
```
vagrant plugin install vagrant-vbguest
vagrant plugin install vagrant-docker-compose
```

5. Fire up the vagrant machine (this should take a while the first time)
```
vagrant up
```

6. Conect to the machine and test
```
vagrant ssh
```