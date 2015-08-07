# inf520

Configuraçõess e documentação do ambiente proposto para inf520.

-----------------------------------------------------------------------

beastie - Iptables fazendo nat para a wan, forwarding intraredes, proxy(Tinyproxy) para controle de acesso, dns recursivo(Unbound) para utilização das redes internas e dhcp v4/v6 (ISC Dhcp Server) para atribuição de endereço na rede clientes. 
status - ok.

eth0 - nat
10.0.2.15

eth1 - mgmt
192.168.56.1/24
fc00:192:168:56::1/64

eth2 - servidores
10.0.69.1/24
fc00:10:0:69::1/64

eth3 - clientes
10.69.0.1/24
fc00:10:0:69::1/64

-----------------------------------------------------------------------

rita - NFS para armazenamento do servidor de logs e MySQL centralizado.
status - ok.

eth0 - mgmt
192.168.56.2/24
fc00:192:168:56::2/64

eth1 - servidores
10.0.69.2/24
fc00:10:0:69::2/64

-----------------------------------------------------------------------

maria - Icinga(baseado em nagios) para monitamento de ativos, Cacti para gerar gráficos(dados) via rrdtool e servidor de logs centralizado via rsyslogd.
statis - ok

eth0 - mgmt
192.168.56.3/24
fc00:192:168:56::3/64

eth1 - servidores
10.0.69.3/24
fc00:10:0:69::3/64

-----------------------------------------------------------------------

madalena - Servidor web nginx e mail(postfix e courie-imap).
status - ok

eth0 - mgmt
192.168.56.4/24
fc00:192:168:56::4/64

eth1 - servidores
10.0.69.4/24
fc00:10:0:69::4/64

-----------------------------------------------------------------------

joaquina - Coletor netflow.
status - ok

eth0 - mgmt
192.168.56.5/24
fc00:192:168:56::5/64

eth1 - servidores
10.0.69.5/24
fc00:10:0:69::5/64

-----------------------------------------------------------------------

helena - DNS autoritativo.
status - ok

eth0 - mgmt
192.168.56.6/24
fc00:192:168:56::6/64

eth1 - servidores
10.0.69.6/24
fc00:10:0:69::6/64

-----------------------------------------------------------------------

cliente - Cliente para teste dos serviços.

eth0 - mgmt
192.168.56.7/24
fc00:192:168:56::7/64

eth1 - servidores
dhcp/dhcp6

-----------------------------------------------------------------------

#eof
