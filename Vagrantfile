Vagrant.configure("2") do |config|
  
  config.vm.define "ans" do |ans|
  
    ans.vm.box="centos/7"
    ans.vm.hostname="ansible"
    ans.vm.network "private_network", ip: "10.0.0.100"
    #ans.vm.synced_folder "./", "/home/vagrant"
  end  

  config.vm.define "web" do |web|

    web.vm.box="centos/7"
    web.vm.hostname="webserver"
    web.vm.network "private_network", ip: "10.0.0.101"
  end  

  config.vm.define "db" do |db|

    db.vm.box="centos/7"
    db.vm.hostname="database"
    db.vm.network "private_network" , ip: "10.0.0.102"
  end  

  config.vm.define "lb" do |lb|

    lb.vm.box="centos/7"
    lb.vm.hostname="loadbalancer"
    lb.vm.network "private_network" , ip: "10.0.0.103"
  end

end