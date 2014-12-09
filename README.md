This Ansible playbook will provide a complete set of firewall rules for any Linux distro that uses iptables(which should be most of them). For RedHat-based distros, the rules file will be put in the canonical location of /etc/sysconfig. For all other distros, it will reside in /etc.

Potential improvements/notes:
-ports 80/443 may not be needed for every machine, these could possibly be removed from the default rules
-ensure rules are loaded on startup across various distros
-add protocol to the data structure, as it currently assumes each rule is for TCP