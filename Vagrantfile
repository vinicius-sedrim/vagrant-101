# -*- mode: ruby -*-
# vi: set ft=ruby :
VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
config.ssh.insert_key = false
config.vm.provider :virtualbox do |vb|
vb.customize ["modifyvm", :id, "--memory", "256"]
 end

 # Criação do Servidor1
 config.vm.define "server1" do |app|
 app.vm.box = "ubuntu/trusty64"
 app.vm.network :private_network, ip: "172.17.177.40"
 end

 # Criação do Servidor2
 config.vm.define "server2" do |app|
 app.vm.box = "ubuntu/trusty64"
 app.vm.network :private_network, ip: "172.17.177.50"
 end

 end