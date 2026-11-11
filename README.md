# jumpbox-setup-ansible

This playbook will setup a jump-server on a freshly installed OpenSUSE MicroOS.

Given there is a freshly installed OpenSUSE MicroOS with:

- `root` user configured during installation.
- network
  - NetworkManager is selected as network stack.
  - Connected only to a trusted network.
  - Can access network to install packages and updates.
- SSH
  - Can SSH into root user with password authentication
 
This playbook will:

- Install required packages and updates.
- Create normal user (specify in config).
- Configure network.
- Configure SSHd
  - Add publickey to normal user.
  - Apply SSHd config
- Configure firewalld.
- Connect to BYOV(Bring Your Own VPN) for remote access.

## Directory Tree

- jumpbox-setup-ansible/
 
## Configuration

