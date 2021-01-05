# Administrative (fill in your information)
  - username: azureadmin
  - web-1 IP = 10.0.0.5
  - web-2 IP = 10.0.0.6
  - web-3 IP = 10.0.0.7
  - My Public IP: 69.217.138.43
  - Jumpbox public IP: 13.82.151.178
  - Jumpbox private IP: 10.0.0.4
  - container name: nifty_galois
  -ELK-VM Public IP: 40.122.147.12
  -ELK-VM Private IP: 10.1.0.4

# Command to display public key
  ls .ssh/
  cat .ssh/id_rsa.pub

# SSH into Jumpbox
  ssh <username>@<jumpboxPUBLICip>
# List all containers
  sudo docker container list -a
# Start a container  
  sudo docker start <container_name>
# Attach (connect to) container
  sudo docker attach <container_name>
# Files underneath container
  /etc/ansible/hosts
  /etc/ansible/ansible.cfg
  
# Ping to verify all is up
  ansible all -m ping

