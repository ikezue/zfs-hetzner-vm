# zfs-hetzner-vm

[![shellcheck](https://github.com/terem42/zfs-hetzner-vm/actions/workflows/shellcheck.yml/badge.svg)](https://github.com/terem42/zfs-hetzner-vm/actions/workflows/shellcheck.yml)

Scripts to install Debian 11, 10 or Ubuntu 18 LTS, 20 LTS, 22 LTS with ZFS root on Hetzner root servers (virtual and dedicated).<br/>
__WARNING:__ all data on the disk will be destroyed.

## How to use:

* Login into Hetzner cloud server console.
* Choose "rescue" menu.
* Click "enable rescue and power cycle", add SSH key to the rescue console, set it OS to linux64, then press mount rescue and power cycle" button.
* connect via SSH to rescue console, and run the script from this repo.

Debian 10 minimal setup with SSH server

````bash
curl -s https://raw.githubusercontent.com/cinderblock/zfs-hetzner-vm/master/hetzner-debian10-zfs-setup.sh | bash -
````

Debian 11 minimal setup with SSH server

````bash
curl -s https://raw.githubusercontent.com/cinderblock/zfs-hetzner-vm/master/hetzner-debian11-zfs-setup.sh | bash -
````

Ubuntu 18.04 LTS minimal setup with SSH server

````bash
curl -s https://raw.githubusercontent.com/cinderblock/zfs-hetzner-vm/master/hetzner-ubuntu18-zfs-setup.sh | bash -
````

Ubuntu 20 LTS minimal setup with SSH server

````bash
curl -s https://raw.githubusercontent.com/cinderblock/zfs-hetzner-vm/master/hetzner-ubuntu20-zfs-setup.sh | bash -
````

Ubuntu 22 LTS minimal setup with SSH server

````bash
curl -s https://raw.githubusercontent.com/cinderblock/zfs-hetzner-vm/master/hetzner-ubuntu22-zfs-setup.sh | bash -
````

Answer script questions about desired hostname and ZFS ARC cache size.

Upon successful run, the script will reboot system, and you will be able to login into it, using the same SSH key you have used within rescue console
