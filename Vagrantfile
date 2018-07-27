boxes = [
  {:name => "IE10-Win7", :box => "http://aka.ms/ie10.win7.vagrant"},
  {:name => "IE10-Win8", :box => "http://aka.ms/ie10.win8.vagrant"},
  {:name => "IE11-Win7", :box => "http://aka.ms/ie11.win7.vagrant"},
  {:name => "IE11-Win8.1", :box => "http://aka.ms/ie11.win81.vagrant"},
  {:name => "IE8-Win7", :box => "http://aka.ms/ie8.win7.vagrant"},
  {:name => "IE9-Win7", :box => "http://aka.ms/ie9.win7.vagrant"},
  {:name => "edge-Win10", :box => "http://aka.ms/msedge.win10.vagrant"}
]

Vagrant.configure(2) do |config|
  boxes.each do |box|
    config.vm.synced_folder ".", "/vagrant", id: "vagrant-root", disabled: true
    config.vm.define box[:name], autostart: false do |machine|
      machine.vm.box = box[:box]
    end
  end
end
