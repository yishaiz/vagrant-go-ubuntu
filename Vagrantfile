# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/trusty64"

    # set the hostname
    config.vm.hostname = "go.dev"

    #provision the box
    config.vm.provision "shell", path: "provision-go.sh"
    config.vm.provision "shell", path: "provision-docker.sh"

    #port forwarding
    config.vm.network "forwarded_port", guest: 8000, host: 7000
	
end


#set the shared folder
#config.vm.synced_folder "src", "/home/vagrant/workspace/src"
    
	