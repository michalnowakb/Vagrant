Vagrant.configure("2") do |config|

  config.vm.define "web" do |web|
  web.vm.box = "ubuntu/xenial64"
  web.vm.network "private_network", ip: "192.168.10.100"
  # web.vm.synced_folder "app", "/home/vagrant/app"
  # web.vm.provision "shell", path: "app/provision.sh"
  end

  config.vm.define "db" do |db|
    db.vm.box = "ubuntu/xenial64"
    db.vm.provision "shell", path: "mongoDB/provision_db.sh"
    
  end

end




