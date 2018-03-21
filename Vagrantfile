Vagrant.configure(2) do |config|
  config.vm.box = "bento/debian-9.3"
  config.vm.provider "virtualbox" do |v|
    v.memory = 8192
    v.cpus = 8
  end
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "provision.yml"
  end
end
