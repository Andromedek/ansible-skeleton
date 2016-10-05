# -*- mode: ruby -*-
# vim: ft=ruby

# Vagrant setup and provisionning. 
Vagrant.configure(2) do |config|
  config.vm.box         = "centos/7"  # more boxes : https://atlas.hashicorp.com/boxes/search
  config.ssh.pty        = true
  config.ssh.insert_key = true

  config.vm.provision "shell",
    :path => "vagrant_specs.sh",
    :upload_path => "/home/vagrant/specs",

    # change role name below
    :args => "--install myrole"
end