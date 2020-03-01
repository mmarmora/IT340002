Vagrant.configure("2") do |config|
  config.vm.define "test_1" do |vm1|
    vm1.vm.box = "bento/ubuntu-18.04"
    vm1.vm.network "public_network"

    vm1.vm.provider "virtualbox" do |vb|
      vb.name = "test_1"
      vb.memory = "512"
    end

    vm1.vm.provision "shell", inline: <<-SHELL
      echo "Hello"
    SHELL
  end

  config.vm.define "test_2" do |vm2|
    vm2.vm.box = "bento/ubuntu-18.04"
    vm2.vm.network "public_network"

    vm2.vm.provider "virtualbox" do |vb|
      vb.name = "test_2"
      vb.memory = "512"
    end

    vm2.vm.provision "shell", inline: <<-SHELL
      echo "Hello"
    SHELL
  end

end
