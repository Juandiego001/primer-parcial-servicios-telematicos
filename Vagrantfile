Vagrant.configure("2") do |config|
 if Vagrant.has_plugin? "vagrant-vbguest"
 config.vbguest.no_install = true
 config.vbguest.auto_update = false
 config.vbguest.no_remote = true
 end
 config.vm.define :cliente do |cliente|
 cliente.vm.box = "centos/stream8"
 cliente.vm.network :private_network, ip: "192.168.56.2"
 cliente.vm.hostname = "cliente"
 end
 config.vm.define :servidor do |servidor|
 servidor.vm.box = "centos/stream8"
 servidor.vm.network :private_network, ip: "192.168.56.3"
 servidor.vm.hostname = "servidor"
 end
 config.vm.define :redireccion do |redireccion|
 redireccion.vm.box = "centos/stream8"
 redireccion.vm.network :private_network, ip: "192.168.56.4"
 redireccion.vm.hostname = "redireccion"
 end
end