# Monit configs for Vesta CP on Centos 7
Services for monitoring:
* crond
* exim
* httpd
* memcached
* mysql
* nginx
* sshd
* vesta-nginx
* vesta-php
* vsftpd

Installation:

    cd /etc/monit.d/
    git clone https://github.com/shapilokk/vesta-centos7-monit.git ./ && rm -f README.md
    /bin/systemctl restart monit


Check service status:

    monit status


If memcached doesn't exist on your system, remove memcached.conf
