Vagrant.configure("2") do |config|
  config.vm.box = "peru/ubuntu-18.04-desktop-amd64"

  config.vm.provider "virtualbox" do |v|
    v.gui = true
  end


  config.vm.provision "shell",
    inline: "sudo apt-get install -y python"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
  end

end
