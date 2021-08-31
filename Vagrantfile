Vagrant.configure("2") do |config|
  ## Node1
  config.vm.define "node1" do |node1|
    node1.vm.provider "virtualbox" do |vb_node1|
      vb_node1.memory = 1024
      vb_node1.cpus = 1
    end
    node1.vm.box = "gusztavvargadr/docker-linux"
    config.vm.synced_folder "./vagrant_data", "/vagrant_data"
    node1.vm.hostname = "node1"
    node1.vm.network "private_network", ip: "10.0.0.10"
    node1.vm.provision "shell", inline: <<-SHELL
      apt-get update && apt-get upgrade -y
    SHELL
  end
  ## Node2
  config.vm.define "node2" do |node2|
    node2.vm.provider "virtualbox" do |vb_node2|
      vb_node2.memory = 1024
      vb_node2.cpus = 1
    end
    node2.vm.box = "gusztavvargadr/docker-linux"
    config.vm.synced_folder "./vagrant_data", "/vagrant_data"
    node2.vm.hostname = "node2"
    node2.vm.network "private_network", ip: "10.0.0.11"
    node2.vm.provision "shell", inline: <<-SHELL
      apt-get update && apt-get upgrade -y
    SHELL
  end
  ## Node3
  config.vm.define "node3" do |node3|
    node3.vm.provider "virtualbox" do |vb_node3|
      vb_node3.memory = 1024
      vb_node3.cpus = 1
    end
    node3.vm.box = "gusztavvargadr/docker-linux"
    config.vm.synced_folder "./vagrant_data", "/vagrant_data"
    node3.vm.hostname = "node3"
    node3.vm.network "private_network", ip: "10.0.0.12"
    node3.vm.provision "shell", inline: <<-SHELL
      apt-get update && apt-get upgrade -y
    SHELL
  end
end
