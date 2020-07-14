# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
   config.vm.box = "centos/7"
   config.vm.box_version="2004.01"
   
   config.vm.network "private_network", ip: "192.168.33.10"
 
   config.vm.synced_folder '.','/vagrant', disabled: true
 
   
   config.vm.provision "shell", inline: <<-SHELL
   
   sudo yum -y install centos-release-scl - python3
   sudo yum -y install rh-python36 - python3

   SHELL
 end