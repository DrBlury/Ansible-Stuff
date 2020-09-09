VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.ssh.insert_key = false

  config.vm.define "vagrant1" do |vagrant1|
    vagrant1.vm.box = "ubuntu/trusty64"
    vagrant1.vm.hostname = "vagrant1"
    vagrant1.vm.network :private_network, ip: "10.0.0.11"

    vagrant1.vm.provider "virtualbox" do |v|
      v.memory = 4096
      v.cpus = 1
    end
  end

  config.vm.define "vagrant2" do |vagrant2|
    vagrant2.vm.box = "ubuntu/trusty64"
    vagrant2.vm.hostname = "vagrant2"
    vagrant2.vm.network :private_network, ip: "10.0.0.12"

    vagrant2.vm.provider "virtualbox" do |v|
      v.memory = 4096
      v.cpus = 1
    end
  end

  config.vm.define "vagrant3" do |vagrant3|
    vagrant3.vm.box = "ubuntu/trusty64"
    vagrant3.vm.hostname = "vagrant3"
    vagrant3.vm.network :private_network, ip: "10.0.0.13"

    vagrant3.vm.provider "virtualbox" do |v|
      v.memory = 4096
      v.cpus = 2
    end
  end
  
end