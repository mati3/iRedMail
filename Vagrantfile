# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-18.04"

  config.vm.network "private_network", ip: "192.168.56.102"

  config.vm.provision "ansible" do |ansible|
      ansible.sudo = true
      ansible.playbook = "playbook.yml"
      ansible.verbose = "v"
      ansible.host_key_checking = false
  end

end
