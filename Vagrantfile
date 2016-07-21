Vagrant.configure(2) do |config|

  config.vm.box = "centos/7"

  # 请安装 vagrant-hostmanager 插件
  # https://github.com/devopsgroup-io/vagrant-hostmanager
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true
  config.hostmanager.manage_guest = true

  config.vm.define "node1" do |node1|
    node1.vm.network "private_network", ip: "192.168.33.11"
    node1.vm.hostname="node1"
  end

  config.vm.define "node2" do |node2|
    node2.vm.network "private_network", ip: "192.168.33.12"
    node2.vm.hostname="node2"
  end

  config.vm.define "node3" do |node3|
    node3.vm.network "private_network", ip: "192.168.33.13"
    node3.vm.hostname="node3"
  end

end
