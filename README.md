# Ansible Playbooks
Those playbooks are made for Ubuntu and Rocky linux to udpate the host system and setup a nginx server with the help of Jinia2 templates.

# Getting Started
1. First go into the directorie of the repo.
2. Now edit the file called inventory, and add in your own hostname or IP address.
3. I'm going to assume that Ansible installed on the system, now let's get to the fun part and run the playbook.
4. There are 2 in the top of the dir, one called deploy_nginx_apt.yml and the other called deploy_nginx_dnf.yml. For example, you have a Ubuntu system run the deploy_nginx_apt.yml, if you have a REHL system that uses dnf run the deploy_nginx_dnf.yml. I'm testing this on a RHEL system for this example.
5. The command is (ansible-playbook deploy_nginx-dnf.yml -i inventory -l rocky). After it's done running and no errors occurred, you should be able to see the webpage be deployed. you can get there using "http://YOUR-IP-HERE/index.html".
