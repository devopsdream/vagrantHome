# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
#web server
  config.vm.define "web" do |web|
     web.vm.box = "hashicorp/precise64"
     web.vm.hostname = "web"
     web.vm.network "private_network", ip:"192.168.50.2"   
     web.vm.provider "virtualbox" do |v|
       v.memory = 1024
       v.cpus = 2
     end
  end
### database
  config.vm.define "db" do |db|
     db.vm.box = "hashicorp/precise64"
     db.vm.hostname = "db"
     db.vm.network "private_network", ip:"192.168.50.3"
     db.vm.provider "virtualbox" do |v|
       v.memory = 512
       v.cpus = 2
     end
  end
end
