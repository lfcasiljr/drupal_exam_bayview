# drupal_exam_bayview
Ansible playbook to install Drupal8, php-fpm and Mariadb softwares on a CentOS 7 machine.
Details requirements:


1. Drupal code should be served via php-fpm and nginx web server.

2. Database to be used for Drupal can be co-hosted on the server, or can be running on a different server.

3. Can be a MySQL or sqlite database.

4. Optimize nginx, php-fpm configuration for a high traffic website. All such configurations should be done via Ansible.

5. Scripts should be executable on a server running SELINUX in enforcing mode, and firewalld enabled

6. Make sure server and other web server configs are hardened security wise.

How to run the playbook:
ansible-playbook -i hosts.txt main.yml --ask-pass --ask-sudo-pass
