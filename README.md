# Monit configs for Vesta CP on CentOS 7
## Services for monitoring:
* clamd
* crond
* dovecot
* exim
* httpd
* memcached
* mysql
* nginx
* spamassassin
* sshd
* vesta-nginx
* vesta-php
* vsftpd

## Other features
* Monitors space and inodes on /
* Monitors system resources (RAM, swap, CPU, load)

## Installation (assuming monit is already installed):

    cd /etc/monit.d/
    git clone https://github.com/infinitnet/vesta-centos7-monit.git ./ && rm -f README.md
    systemctl restart monit

## Check service status:

    monit <status|summary>

