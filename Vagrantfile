# -*- mode: ruby -*-
# vi: set ft=ruby :

PROJECT_NAME = "wishjob"

Vagrant.configure(2) do |config|
  config.vm.box = "aspyatkin/ubuntu-16.04-server-amd64"
  config.vm.hostname = PROJECT_NAME

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

  config.vm.synced_folder ".", "/home/vagrant/" + PROJECT_NAME

  ENV["LC_ALL"] = "en_US.UTF-8"

  config.vm.network "forwarded_port", guest: 8080, host: 8080
end
