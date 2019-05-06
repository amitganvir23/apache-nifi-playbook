# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7.6"
  config.vm.hostname = "nifi.example.com"
  config.vm.network "private_network", ip: "192.168.33.10"

  # config.vm.synced_folder "./data", "/vagrant", type: "nfs"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "./ansible/playbook.yml"
  end
end
