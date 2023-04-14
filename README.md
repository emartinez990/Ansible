# Ansible Cisco Network Check 
#Ansible version
ansible 2.9.6
  config file = /etc/ansible/ansible.cfg
  configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/lib/python3/dist-packages/ansible
  executable location = /usr/bin/ansible
  python version = 3.8.10 (default, Mar 13 2023, 10:26:41) [GCC 9.4.0]
#paramiko additionally installed
apt-get install -y python3-paramiko
#ansible.cfg - modified the following to disable host key checking
host_key_checking = False

#Ansible Tree
.
├── ansible.cfg
├── hosts
├── inventory
│   ├── group_vars
│   │   └── switches
│   │       ├── switches.yml
│   │       └── vault
│   ├── host_file
│   └── host_file.bak
└── playbooks
    ├── cisco_switch_netcheck.yml
    └── show_version.yml
