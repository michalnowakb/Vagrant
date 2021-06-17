Vagrant.configure("2") do |config|

  config.vm.define "web" do |web|
  web.vm.box = "ubuntu/xenial64"
  web.vm.network "private_network", ip: "192.168.10.100"
  # web.hostsupdater.aliases = ["development.local"]
  web.vm.synced_folder "app", "/home/vagrant/app"
  web.vm.provision "shell", path: "app/provision.sh"
  end

  config.vm.define "db" do |db|
  db.vm.box = "ubuntu/xenial64"
  db.vm.network "private_network", ip: "192.168.10.123"
  # web.hostsupdater.aliases = ["database.local"]
  db.vm.synced_folder "mongoDB", "/home/ubuntu/environment" 
  db.vm.provision "shell", path: "mongoDB/provision_db.sh"

    
  end

end




