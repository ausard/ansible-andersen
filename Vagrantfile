Vagrant.configure("2") do |config|
  config.vm.define "web01" do |web01|
    web01.vm.box = "bento/ubuntu-16.04"
    web01.vm.network "private_network", ip: "192.168.33.11"
    web01.vm.hostname = "web01"
    web01.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
    web01.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end
end
