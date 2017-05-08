VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(2) do |config|
  config.vm.define "web" do |web|
   web.vm.box = "precise32"
   web.vm.hostname = 'web'
   web.vm.network :private_network, ip: "192.168.56.101"
   web.vm.box_url = "precise32"


  web.vm.provision :ansible do |ansible|
   ansible.playbook = "playbook.yml"
  
  end
  end
end
