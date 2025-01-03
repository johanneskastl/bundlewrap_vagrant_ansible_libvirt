# bundlewrap_vagrant_libvirt_ansible

This Vagrant setup creates a VM and installs
[Bundlewrap](https://bundlewrap.org/).

Default OS is openSUSE Tumbleweed. Although that can be changed in the
Vagrantfile, please beware that this will break the Ansible provisioning.

## Vagrant

1. You need vagrant obviously. And ansible. And git...
1. Fetch the box, per default this is `opensuse/Tumbleweed.x86_64`, using
   `vagrant box add opensuse/Tumbleweed.x86_64`.
1. Make sure the git submodules are fully working by issuing `git submodule init
   && git submodule update`
1. Run `vagrant up`
1. Log in using `vagrant ssh`. The `vagrant` user has a SSH key (with an empty
   passphrase) so it can log in on the VM itself using `ssh localhost`.
1. Check the [quickstart
   tutorial](https://docs.bundlewrap.org/guide/quickstart/) and start playing
   around with bundlewrap.
1. Party!

## Cleaning up

The VMs can be torn down after playing around using `vagrant destroy`.

## License

BSD-3-Clause

## Author Information

I am Johannes Kastl, reachable via git@johannes-kastl.de
