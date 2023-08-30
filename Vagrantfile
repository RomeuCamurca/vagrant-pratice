Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.provision :shell, path: "script.sh"
  config.vm.network "private_network", ip: "10.0.2.15"
  config.vm.network "public_network", ip: "192.168.0.17"
  config.vm.network :forwarded_port, guest: 80, host: 8080
  config.vm.synced_folder "/Users/Romeu/Desktop/IT-Talent-2023.2/vagrant/templates/", "/srv/website"
end
