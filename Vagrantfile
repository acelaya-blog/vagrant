Vagrant.configure("2") do |config|

    # This is the operating system to be installed. Ubuntu 12.04 in this case
    config.vm.box = "hashicorp/precise32"

    # The script "bootstrap.sh" will we run within the virtual machine once installed
    config.vm.provision :shell, path: "bootstrap.sh"

    # The port 8888 will be forwarded from the local machine to the virtual machine's port 80
    config.vm.network :forwarded_port, host: 8888, guest: 80

end
