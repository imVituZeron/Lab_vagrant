Vagrant.configure("2") do |config|
    # criando uma VM ubuntu com o hostname lab, rede publica pegando a bridge
    # do host, e executando o script dentro da VM.
    config.vm.box = "ubuntu/trusty64"
    config.vm.hostname = "lab"
    config.vm.network "public_network", bridge: "enp2s0"
    config.vm.provision "shell", path: "script.sh"
end