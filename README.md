# Ansible - Cisco Automation Network
Cisco Automation Network - Config Cisco device with Ansible

Prerequisites:
* Ansible 2.10 (or higher) installed: [installation_guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
* Cisco Device can remote access by SSH / Telnet
* Network platform: cisco.ios 
* Communication Protocol: ansible.netcommon.network_cli

## CONFIG CISCO SWITCH
Modules List:
* Change Hostname
* Change Password (this module change password enable, user/pass login, password ssh)
* Create Vlan (this module add vlan, change vlan name, replace vlan, delete vlan)
* Config Interface ( this module change description, add/replace vlan to interface, config access/trunk port...)
* Config SNMP (SNMP monitoring can be used to collect information)
* Save Config (command "write" to save running-config => startup-config)

## Usage
```ansible
ansible-playbook config_switch_cisco.yml
```

## Roadmap
* Import .csv file
* Manage Layer3 interfaces on Cisco IOS network devices
* Add more modules to this playbook
## Authors
-DuLaP-
