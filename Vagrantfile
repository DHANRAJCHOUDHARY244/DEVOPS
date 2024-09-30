Vagrant.configure("2") do |config|
  # Define the scriptbox virtual machine
  config.vm.define "scriptbox" do |scriptbox|
    scriptbox.vm.box = "generic/centos7"
    scriptbox.vm.network "private_network", ip: "192.168.10.12"
    scriptbox.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Define the web01 virtual machine
  config.vm.define "web01" do |web01|
    web01.vm.box = "generic/centos7"
    web01.vm.network "private_network", ip: "192.168.10.13"
    web01.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Define the ubuntu virtual machine
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/bionic64"
    ubuntu.vm.network "private_network", ip: "192.168.10.1"
    ubuntu.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Define the web02 virtual machine
  config.vm.define "web02" do |web02|
    web02.vm.box = "generic/centos7"
    web02.vm.network "private_network", ip: "192.168.10.14"
    web02.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Define the web03 virtual machine (CentOS)
  config.vm.define "web03" do |web03|
    web03.vm.box = "generic/centos7"
    web03.vm.network "private_network", ip: "192.168.10.15"
    web03.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
end
