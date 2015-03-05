# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  # Define the base box to use
  config.vm.box = "ubuntu/trusty64"

  # Forward port 80 on the guest as 1337 on the host
  config.vm.network "forwarded_port", guest: 80, host: 1337

  # Mount working directory as www-data
  config.vm.synced_folder ".", "/vagrant", owner: "www-data", group: "www-data"

  # Allow SSH agent forwarding
  config.ssh.forward_agent = true

  # Virtualbox configuration
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--memory", "1024"]
  end

  # Provisioner configuration
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
  end

end
