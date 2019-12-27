Vagrant.configure("2") do |config|
  config.vm.define "web01" do |web01|
    web01.vm.box = "ubuntu/bionic64"
    web01.vm.network "private_network", ip: "192.168.33.11"
    web01.vm.hostname = "web01"
    web01.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end    
  end
end
