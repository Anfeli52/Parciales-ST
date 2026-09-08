# -- mode: ruby --
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
        config.vm.define :servidorMaestro do |servidorMaestro|
                servidorMaestro.vm.box = "bento/ubuntu-22.04"
                servidorMaestro.vm.network :private_network, ip: "192.168.58.3"
                servidorMaestro.vm.hostname = "servidorMaestro"
        end
        config.vm.define :servidorEsclavo do |servidorEsclavo|
                servidorEsclavo.vm.box = "bento/ubuntu-22.04"
                servidorEsclavo.vm.network :private_network, ip: "192.168.58.2"
                servidorEsclavo.vm.hostname = "servidorEsclavo"
        end
	config.vm.define :cliente do |cliente|
		cliente.vm.box = "bento/ubuntu-22.04"
		cliente.vm.network :private_network, ip: "192.168.58.10"
		cliente.vm.hostname = "cliente"
	end
	config.vm.define :servidorWeb do |servidorWeb|
		servidorWeb.vm.box = "bento/ubuntu-22.04"
		servidorWeb.vm.network :private_network, ip: "192.168.58.4"
		servidorWeb.vm.hostname = "servidorWeb"
	end
end
