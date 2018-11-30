# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.provider 'virtualbox' do |vb|
      vb.gui = false
      vb.memory = '512'
      vb.cpus = 2
    end
    config.vm.box = "ubuntu/xenial64"
    config.vm.network "forwarded_port", guest: 80, host: 80
    config.vm.boot_timeout = 6000

    config.vm.provision "shell", inline: <<-SHELL
        apt-get -y update
        apt-get install -y nginx

    SHELL

end
