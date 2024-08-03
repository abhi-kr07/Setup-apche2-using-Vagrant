# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "web-server"
  config.vm.hostname = "web-server"
  config.vm.box = "bento/ubuntu-20.04"

  config.vm.network "forwarded_port", guest: 80 , host: 8080 , host_ip: "<local-ip-addr>"

  config.vm.synced_folder "./html/", "/var/www/html"

  # config.vm.synced_folder ".", "/vagrant", disabled: true

  config.vm.provider "virtualbox" do |vb|
    vb.name = "web-server"
    # Display the VirtualBox GUI when booting the machine
    vb.gui = false
  
    # Customize the amount of memory on the VM:
    vb.memory = "2048"
  end
  

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y apache2
  SHELL
  config.vm.provision "shell", run: "always", inline: <<-SHELL
    echo "Hello Abhishek , This is your Vagrantfile"
  SHELL

end
