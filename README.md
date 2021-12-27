# Vagrant Boxes

## Supported Boxes and Respective Packer Template Links

  - [`hbasria/ubuntu-20.04`](https://app.vagrantup.com/hbasria/boxes/ubuntu-20.04-server)
      - [`ubuntu-server/libvirt-20.04/packer.json`](https://github.com/hbasria/packer-boxes/blob/master/ubuntu-server/libvirt-20.04/packer.json)

## Overview

  - Packaging with [Packer](https://www.packer.io/)
  - Minimal [Vagrant base box implementation](https://www.vagrantup.com/docs/boxes/base)
  - Support [QEMU Guest Agent](https://wiki.qemu.org/Features/GuestAgent)
  - Support [Vagrant synced folder with rsync](https://www.vagrantup.com/docs/synced-folders/rsync)
  - Standardize disk partition with GPT
  - Standardize file system mount with UUID
  - Standardize network interface with `eth0`

### Quick Start

Once you have [Vagrant](https://www.vagrantup.com/docs/installation) and [VirtaulBox](https://www.virtualbox.org/) installed, run the following commands under your [project directory](https://learn.hashicorp.com/tutorials/vagrant/getting-started-project-setup?in=vagrant/getting-started):

    # Initialize Vagrant
    vagrant init hbasria/ubuntu-20.04-server
    
    # Start the virtual machine
    vagrant up
    
    # SSH into this machine
    vagrant ssh
    
    # Terminate the virtual machine
    vagrant destroy --force

## Versioning

## License

  - Code released under [MIT License](LICENSE)

