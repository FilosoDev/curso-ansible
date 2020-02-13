VAGRANTFILE_API_VERSION = "2"
ENV['VAGRANT_DEFAULT_PROVIDER'] = 'libvirt'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = "generic/debian10"
    config.vm.hostname = "curso"
    config.vm.define :"workstation" 
    config.vm.network :private_network, ip: "192.168.1.20"
    config.ssh.insert_key = false

    config.vm.provider :libvirt do |v|
      v.memory = 1024
      v.cpus = 1
    end
end
