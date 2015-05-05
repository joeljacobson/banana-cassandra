# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "precise64"
    config.vm.box_url = "http://files.vagrantup.com/precise64.box"

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "site.yml"
        end

        config.vm.provider "virtualbox" do |vb|
   vb.customize ["modifyvm", :id, "--memory", "8196"]
 end

end
