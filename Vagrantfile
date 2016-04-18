boxes = [
  {:name => "IE10-Win7", :box => "modernIE/w7-ie10"},
  {:name => "IE10-Win8", :box => "modernIE/w8-ie10"},
  {:name => "IE11-Win7", :box => "modernIE/w7-ie11"},
  {:name => "IE11-Win8.1", :box => "modernIE/w8.1-ie11"},
  {:name => "IE8-Win7", :box => "modernIE/w7-ie8"},
  {:name => "IE9-Win7", :box => "modernIE/w7-ie9"}
  {:name => "edge-Win10", :box => "Microsoft/EdgeOnWindows10"}
]

Vagrant.configure(2) do |config|
  boxes.each do |box|
    config.vm.synced_folder ".", "/vagrant", id: "vagrant-root", disabled: true
    config.vm.define box[:name], autostart: false do |machine|
      machine.vm.box = box[:box]
    end
  end
end
