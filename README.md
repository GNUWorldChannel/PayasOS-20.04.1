# PayasOS-20.04.1 server.

request us access to download it
via: https://drive.google.com/file/d/1UKf2fZHSWD53P-S5IgKslgXVNp-ewBgY/view?usp=sharing

This is a VM image created under Virtual Box, uncompress and run it.
--- Ubuntu 20.04.1 server, installed with IRCU and GNUWORLD. ---

ssh port: 22 Destination ip: check your DHCP and if you want
a static one, go /etc/netplan and look the file "static-readme".

NOTE: The first boot could take a while when your OS is
getting your network adapter configuration.
We tested the network configuration, so let it as bridge
do not change it to NAT. Always check your adapter 
name there.

------------------------------------------
Users created: 

sudo user: anaconda
password: vaiacondios

root user
password: vaiacondios

(where is ircd / gnuworld)

gnuworld user
password: vaiacondios

------------------------------------------
Once you edit ircd.conf, GNUWorld.conf
cservice.conf and ccontrol.conf files.
you can start ircd + gnuworld using
./runall.sh file located at home in
gnuworld user :).

X login has "admin" as 1000 and the password
is temPass as usual.

If you want a custom 1000, then add it into the db
using the script as user id 2. 

------------------------------------------

If you have any question please read our guide
https://github.com/GNUWorldChannel/Installation-guide

-Review- y2k/ARI3L
