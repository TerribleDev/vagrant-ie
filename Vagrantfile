boxes = [
  {:name => "IE10-Win7", :box => "https://az792536.vo.msecnd.net/vms/VMBuild_20150916/Vagrant/IE10/IE10.Win7.Vagrant.zip"},
  {:name => "IE11-Win7", :box => "https://az792536.vo.msecnd.net/vms/VMBuild_20150916/Vagrant/IE11/IE11.Win7.Vagrant.zip"},
  {:name => "IE11-Win8.1", :box => "https://az792536.vo.msecnd.net/vms/VMBuild_20150916/Vagrant/IE11/IE11.Win81.Vagrant.zip"},
  {:name => "IE8-Win7", :box => "https://az792536.vo.msecnd.net/vms/VMBuild_20150916/Vagrant/IE8/IE8.Win7.Vagrant.zip"},
  {:name => "IE9-Win7", :box => "https://az792536.vo.msecnd.net/vms/VMBuild_20150916/Vagrant/IE9/IE9.Win7.Vagrant.zip"},
  {:name => "edge-Win10", :box => "https://az792536.vo.msecnd.net/vms/VMBuild_20180425/Vagrant/MSEdge/MSEdge.Win10.Vagrant.zip"}
]

Vagrant.configure(2) do |config|
  boxes.each do |box|
    config.vm.synced_folder ".", "/vagrant", id: "vagrant-root", disabled: true
    config.vm.define box[:name], autostart: false do |machine|
      machine.vm.box = box[:box]
    end
  end
end
