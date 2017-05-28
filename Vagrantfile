# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.provider :vultr do |vultr, override|
    override.ssh.private_key_path = '~/.ssh/id_rsa'
    override.vm.box = 'vultr'
    override.vm.box_url = 'https://github.com/p0deje/vagrant-vultr/raw/master/box/vultr.box'

    vultr.token = ENV['VULTR_API_KEY']
    vultr.region = 'Tokyo'
    vultr.plan = '1024 MB RAM,25 GB SSD,1.00 TB BW'
    vultr.os = 'Debian 8 x64 (jessie)'
  end
end
