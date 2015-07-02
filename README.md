# inf520

Confs e docs do ambiente.

GW -> beastie -> how to:

apt-get update

apt-get -y install unbound\n
apt-get -y purge bind9
apt-get -y install tinyproxy
apt-get -y install isc-dhcp-server

cp /etc/unbound/unbound.conf.d/unbound.conf /etc/unbound/unbound.conf.d/
cp /etc/tinyproxy.conf /etc/
cp /etc/filter /etc/

