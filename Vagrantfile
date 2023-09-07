Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"
  config.vm.define:app do |app_config|
    app_config.vm.network "public_network", ip: "192.168.0.77"
    
    app_config.vm.provision "shell", inline: "sudo apt-get update && sudo apt-get install -y nginx"
    app_config.vm.provision "shell", inline: "sudo apt-get install -y vim && sudo apt-get install -y curl && sudo atp-get install -y telnet"
    app_config.vm.provision "shell", inline: "sudo apt-get install -y unzip && sudo apt-get install -y wget && sudo atp-get install -y net-tools"
    app_config.vm.provision "shell", inline: "sudo apt-get install -y htop && sudo apt-get install -y nmap && sudo useradd -m -s /sbin/bash GiovaniMarques"
  
    app_config.vm.provider:virtualbox do |v|
      v.name = "VM Vagrant"
    end
  end
end
