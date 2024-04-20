# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "Master" do |master|
    master.vm.box = "ubuntu/focal64"
    master.vm.network "private_network", type: "dhcp"
    master.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end


  end

  config.vm.define "Slave" do |slave|
    slave.vm.box = "ubuntu/focal64"
    slave.vm.network "private_network", type: "dhcp"
    slave.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
    end
  end
end
