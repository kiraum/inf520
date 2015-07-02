# inf520

Confs e docs do ambiente.

GW -> beastie -> how to:

apt-get update
apt-get -y install unbound
cp /etc/unbound/unbound.conf.d/unbound.conf
apt-get -y purge bind9
apt-get -y install tinyproxy
cp /etc/tinyproxy.conf
cp /etc/filter
apt-get -y install isc-dhcp-server
