# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"
  config.vm.network :forwarded_port, host: 5000, guest: 5000
  config.vm.network :private_network, ip: "192.168.111.228"
  config.vm.synced_folder "project", "/home/vagrant/project"
  config.vm.synced_folder "frameworks", "/home/vagrant/frameworks"
  
  config.vm.provision :ansible do |ansible| 
    ansible.limit = 'vagrant'
    ansible.playbook = "provisioning/playbook.yml"
    ansible.inventory_path = "provisioning/ansible_hosts"
  end

end
