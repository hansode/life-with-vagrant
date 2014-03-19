# Setup Vagrant

## [Vagrant](http://www.vagrantup.com/)

> Create and configure lightweight, reproducible, and portable development environments.

## System Requirements

### Windows

+ [Vagrant](http://www.vagrantup.com/downloads.html)
+ [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
+ [VMware Workstation](http://www.vmware.com/jp/products/workstation/)
+ [Vagrant-VMware Lisence](http://www.vagrantup.com/vmware#buy-now)
+ [Cygwin](http://www.cygwin.com/)
  + openssh

### MacOS

+ [Vagrant](http://www.vagrantup.com/downloads.html)
+ [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
+ [VMware Fusion](http://www.vmware.com/jp/products/fusion/)
+ [Vagrant-VMware Lisence](http://www.vagrantup.com/vmware#buy-now)

## Tips

### Cygwin

```
$ ln -s /cygdrive/c/Users/$(whoami)/.vagrant.d ~/
$ ln -s /cygdrive/c/Users/$(whoami)/Documents/Virtual\ Machines ~/VMware\ VMs
```

## Install Vagrant Plugins

### Windows: vagrant-vmware-workstation

```
$ vagrant plugin install vagrant-vmware-workstation
$ vagrant plugin license vagrant-vmware-workstation license.lic
```

### MacOS: vagrant-vmware-fusion

```
$ vagrant plugin install vagrant-vmware-fusion
$ vagrant plugin license vagrant-vmware-fusion license.lic
```

### [vagrant-global-status](http://www.ryuzee.com/contents/blog/6834)

```
$ vagrant plugin install vagrant-global-status
```

## Getting Started

```
$ mkdir -p ~/work/vagrant/sandbox
$ cd       ~/work/vagrant/sandbox

$ vagrant init hansode/centos-6.5-x86_64
$ vagrant up
$ vagrant ssh
```
