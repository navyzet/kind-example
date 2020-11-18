Vagrant.configure("2") do |config|
  config.vm.box = "generic/debian10"
  config.vm.define "devbox.test.com" do |devbox1|
  devbox1.vm.network "forwarded_port", guest: 80, host: 8080
  end
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
