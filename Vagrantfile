Vagrant.configure("2") do |config|
  config.vm.box = "generic/debian10"
  config.vm.define "devbox.test.com" do |devbox1|
  end
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
