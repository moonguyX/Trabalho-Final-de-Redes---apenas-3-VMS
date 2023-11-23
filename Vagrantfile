Vagrant.configure("2") do |config|

  config.vm.define "vm1" do |vm1|
    vm1.vm.box = "http://192.168.24.55/vagrant-boxes/focal64.box"
    vm1.vm.network "forwarded_port", guest: 808, host: 7000
    vm1.vm.network "private_network", ip: "192.168.56.13"

    vm1.vm.synced_folder "./diretorioPC", "/diretorioHost"
 
    vm1.vm.provider "virtualbox" do |vb1|
      vb1.memory = "512"
      vb1.cpus = "1"
    end
  end

  config.vm.define "vm2" do |vm2|
    vm2.vm.box = "http://192.168.24.55/vagrant-boxes/focal64.box"
    vm2.vm.network "forwarded_port", guest: 808, host: 6000
    vm2.vm.network "private_network", ip: "192.168.56.12"

    vm2.vm.synced_folder "./diretorioPC", "/diretorioHost"

    vm2.vm.provider "virtualbox" do |vb2|
      vb2.memory = "512"
      vb2.cpus = "1"
    end
  end

  config.vm.define "vm3" do |vm3|
    vm3.vm.box = "http://192.168.24.55/vagrant-boxes/focal64.box"
    vm3.vm.network "forwarded_port", guest: 808, host: 5000
    vm3.vm.network "private_network", ip: "192.168.56.11"

    vm3.vm.synced_folder "./diretorioPC", "/diretorioHost"

    vm3.vm.provider "virtualbox" do |vb3|
      vb3.memory = "512"
      vb3.cpus = "1"
    end
  end

end