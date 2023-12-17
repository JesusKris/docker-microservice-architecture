# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|

  config.vagrant.plugins = ["vagrant-env"]
  config.env.enable
  config.vm.box = ENV['VAGRANT_BOX']

  config.vm.network "forwarded_port", guest: ENV['EXPRESS_PORT'], host: ENV['EXPRESS_HOST_PORT']


  # Sync the root directory to /vagrant on the guest VM
  config.vm.synced_folder ".", "/vagrant", type: "rsync", rsync__exclude: [
    "Vagrantfile",
    ".gitignore",
    ".vagrant",
  ], rsync__include: [".env", "*"]

  # Provisioner to copy .env file to ./src/api-gateway
  config.vm.provision "file", source: ".env", destination: "/vagrant/src/api-gateway/.env"

  # Provisioner to copy .env file to ./src/billing-app
  config.vm.provision "file", source: ".env", destination: "/vagrant/src/billing-app/.env"

  # Provisioner to copy .env file to ./src/inventory-app
  config.vm.provision "file", source: ".env", destination: "/vagrant/src/inventory-app/.env"

  config.vm.provision "shell", path: "./scripts/setup_docker.sh"

end
