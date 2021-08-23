Vagrant.configure("2") do |dlsinc_lab|
  dlsinc_lab.vm.define "dlsinc_vm" do |dlsinc_vm|
    dlsinc_vm.vm.provider "vmware_desktop" do |v|
     v.cpus = 2
     v.memory = 2048
     v.allowlist_verified = true
    end
    dlsinc_vm.vm.box = "dlsinc/dlsincvm"
    dlsinc_vm.vm.hostname = "dlsincvm.dlsinc.internal"
    dlsinc_vm.vm.network "private_network", ip: "10.100.200.20"
    dlsinc_vm.vm.synced_folder ".", "/vagrant"
  end
end