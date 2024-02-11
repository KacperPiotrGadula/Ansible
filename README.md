# Ansible

## Future is somefing impres and inspirate to be ansible master 

* Write code to add new user to vm
* Write code to install docker and unzip

### Package managment

* apt, yum, pkg, apt_repository - we use 'package'

### Files and directories

* template, file, lineinfile, blockinfile, copy, fetch, and stat

### System

* service, user, group, cron, hostname, autorized_key, intables, modprobe, kernel_blacklist, guster_volume, lvm

### Various Useful

* raw, synchronize, get_url, unarchive, ec2, rds

## Variables
* Variables: Just like the already used programming languages
* Scopes: Global, Per-Play, and Per-Host
* Start with a letter, contain only alphanumerics and underscores
* Registered with 'register'
* Referenced with {{ varname }} syntax
* Dictionary variables can be accessed using regular Python and dot notation
* my.var and my['var']
* Explicitly include a vars YAML file from your playbook:
* include_var: myvars.yml
* Set variables for hosts or host groups in your inventory
* Set role-specific variables in your roles/role name/vars/directory

## Facts
* Facts: information about hosts in your inventory that's gathered by Ansible
when it connects to a host
* You can use these facts in your plays - they are represented as variables stored
in a dictionary
* You can disable fact gathering by setting 'gather_facts: False' at the playbook
level (for example, prepare_ansible_target.yml)
* Gather facts and print to stdout:
    * ansible <host> -m setup -u root