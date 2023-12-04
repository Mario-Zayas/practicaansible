# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|
    config.vm.define :servidorweb do |servidorweb|
      servidorweb.vm.box = "debian/bookworm64"
      servidorweb.vm.hostname = "servidorweb"
      servidorweb.vm.synced_folder ".", "/vagrant", disabled: true
      servidorweb.vm.network :private_network,
          :libvirt__network_name => "red_privada1",
          :libvirt__dhcp_enabled => false,
          :ip => "10.0.0.2",
          :libvirt__forward_mode => "veryisolated"
    end
    
  end
  
