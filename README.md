![1](https://user-images.githubusercontent.com/87182167/134289842-eae3051f-7c4a-4cea-bb51-3525e5088191.jpeg)
# Ansible-Cisco-DevNet

### Command to install Ansible on Ubuntu machine

```
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
ansible --version

```

### Sample hosts or Inventory Settings

```
[routers]
sandbox-iosxe-latest-1.cisco.com

[routers:vars]
ansible_user=developer
ansible_password=C1sco12345
ansible_connection=network_cli
ansible_network_os=ios
ansible_port=22

```

### Update required in ansible.cfg

```
host_key_checking=False

```

