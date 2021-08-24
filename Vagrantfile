# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    ## Vagrant Box
    config.vm.box = "ubuntu/focal64"

    ## Containers
    config.vm.define 'containers' do |containers|
        containers.vm.hostname = "containers"

        # VM Size config
        containers.vm.provider "virtualbox" do |v|
            v.name = "containers"
            v.memory = 1024
            v.cpus = 2
        end

        # VM Config
        containers.vm.provision :ansible_local do |ansible|
            ansible.install_mode = "default"
            ansible.playbook = "ansible/playbook.yml"
            ansible.verbose = true
            ansible.install = true
            ansible.limit = "all"
            ansible.inventory_path = "ansible/inventory"

        end
    end
end