# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "private_network", ip: "10.1.1.1"
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 1
  end

  # config.vm.provision "ansible" do |ansible|
  #   ansible.playbook = "provision-vagrant.yml"
  # end

  config.vm.synced_folder ".", "/vagrant"
end
