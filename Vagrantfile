# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.provider 'virtualbox' do |vb|
      vb.gui = false
      #vb.memory = '512'
      vb.cpus = 1
    end
    config.vm.box = "inviqa/centos-6-stack-php55"
    config.vm.network "forwarded_port", guest: 5000, host: 5000
    config.vm.boot_timeout = 600

end
