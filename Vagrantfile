# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/trusty64"
    config.vm.network "private_network", ip: "192.168.33.30"
    config.vm.network "forwarded_port", guest: 80, host: 8082
    config.vm.network "forwarded_port", guest: 3306, host: 3307
    config.vm.hostname = "ubuntu"
    config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]

end
