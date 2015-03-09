# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "puppetlabs/debian-7.8-64-puppet"
  config.vm.network "private_network", ip: "192.168.33.10"
  config.berkshelf.enabled = true
  config.vm.provision "chef_solo" do |chef|
    chef.roles_path = "roles"
    chef.add_role "web"
  end
end
