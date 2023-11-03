# 📦  Vagrant awesome command line for day by day!

## Intro & Documentation

Vagrant is a tool for building complete development environments. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases development/production parity, and makes the ***"it works on  machine"*** excuse a relic of the past.

***What is Vagrant?***
Vagrant is the command line utility for managing the lifecycle of virtual machines. Isolate dependencies and their configuration within a single disposable and consistent environment.

+ [Official Vagrant Intro][intro]

[intro]: https://developer.hashicorp.com/vagrant/intro

+ [Official Vagrant Docs][doc]

[doc]: https://developer.hashicorp.com/vagrant/docs

+ [Official Vagrant CLI][vcli]

[vcli]: https://developer.hashicorp.com/vagrant/docs/cli

## Main command
+ `vagrant validate` - This command validates your [Vagrantfile](https://developer.hashicorp.com/vagrant/docs/vagrantfile).
+ `vagrant up` - Start all VMs using Vagrantfile (please enter into vagrant-cluster/ folder before run this command)
+ `vagrant status`  - Check the status of the VM's
+ `vagrant ssh vm`  - Open ssh on target VM
+ `vagrant destroy` - Destroy specific instance or destroy all instances, without VM name
+ `vagrant suspend` - A suspend effectively saves the exact point-in-time state of the machine, so that when you resume it later, it begins running immediately from that point, rather than doing a full boot.

## Example with some context

### Copy a file from local to vagrant host machine : 
You need to transfer file or folder from your PC to Vagrant host and you need a solution.
Here some good example summirized :
1. Using vagrant plugin : 

    + `vagrant plugin install vagrant-scp`
    + `vagrant scp /data/examples/spring-boot webserver:/home/vagrant`
        > `vagrant scp <some_local_file_or_dir> [vm_name]:<somewhere_on_the_vm>`

2. Using classic scp command (findout the correct forward port in Virtualbox VM Settings > Network > First adapter > Forwarderd port) : 
    
    + File : `scp -P 2222 /data/examples/spring-boot/gs-spring-boot-master.zip vagrant@127.0.0.1:/home/vagrant` 
    + Folder : `scp -P 2222 -r /data/examples/spring-boot vagrant@127.0.0.1:/home/vagrant`
3. Using Vagrantfile provisioner  

[Reference][refscp]

[refscp]
https://howtoprogram.xyz/2017/08/13/copy-files-folders-host-guest-vagrant/
