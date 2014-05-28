#vagrant setup with scikit-learn, numpy ++

A simple Vagrant config that gets you started quickly. When deployed, the folder structure will look like this: 
- yourrepo/
  - frameworks/
      - ...
  - project/
      - ...
  - provision/
      - templates/
      - ansible_hosts
      - playbook.yml
  - ansible.cfg
  - Vagrantfile


##Requirements

- VirtualBox https://www.virtualbox.org/
- Vagrant http://www.vagrantup.com/  (ATOW version 1.4.3)
- Ansible http://docs.ansible.com/ (ATOW version 1.5)
- Some console knowledge :-)

##Getting Started
    
    git clone git@github.com:torbjokv/vagrant-scikit-learn.git yourrepo && cd yourrepo && vagrant up

This takes time. Grab a coffee - or two!

    vagrant ssh

Le voilà!

##Problems?

Vagrant and ansible have good dokumentation at http://docs.vagrantup.com/v2 and http://docs.ansible.com/
