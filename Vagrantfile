# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
config.vm.define :stream do |stream|
stream.vm.box = "bento/centos-7.9"
stream.vm.network :private_network, ip: "192.168.50.2"
stream.vm.provision "shell", path: "script2.sh"
stream.vm.hostname = "stream"
end

config.vm.define :firewallNAT do |firewallNAT|
firewallNAT.vm.box = "bento/centos-7.9"
firewallNAT.vm.network :private_network, ip: "192.168.50.3"
firewallNAT.vm.provision "shell", path: "script.sh"
firewallNAT.vm.hostname = "firewallNAT"
end
end