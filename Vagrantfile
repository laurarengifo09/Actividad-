# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
 config.vm.define :servidor do |servidor|
 servidor.vm.box = "bento/ubuntu-22.04"
 servidor.vm.network :private_network, ip: "192.168.50.3"
 servidor.vm.network :public_network, ip: "192.168.1.37"
 #servidor.vm.network :public_network, bridge: "ethp", :dhcp => true
 servidor.vm.hostname = "servidor"
 config.vm.synced_folder "./recursos", "/vagrant_data"
 end
 config.vm.define :cliente do |cliente|
 cliente.vm.box = "bento/ubuntu-22.04"
 cliente.vm.network :private_network, ip: "192.168.50.2"
 cliente.vm.hostname = "cliente"
 end
end
