Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise64"

  # Network
  config.vm.network "private_network", ip: "192.168.33.10"

       # Tell Vangrant to use ansible
        config.vm.provision :ansible do |ansible|
       # Where playbook is locate
        ansible.playbook = "provisioning/main.yml"
  end
end
