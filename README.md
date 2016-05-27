# Monit configs for Vesta CP on Centos 7
Installation:
    cd /etc/monit.d/
    git clone https://github.com/shapilokk/vesta-centos7-monit.git
    /bin/systemctl restart monit Check service status:
    monit status
If memcached doesn't exist on your system, remove memcached.conf
