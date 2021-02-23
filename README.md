<p style="text-align:center;"><img src="https://github.com/GNUWorldChannel/PayasOS-20.04.1/blob/main/logo-final.png" alt="PayasOS 20.04.1 by y2k and ARI3L"></p>

# PayasOS-20.04.1 server.

Request us access to download it via:
https://drive.google.com/file/d/1UKf2fZHSWD53P-S5IgKslgXVNp-ewBgY/view?usp=sharing

This is a VM image created under Virtual Box, uncompress, edit mandatory
config files and enjoy :)

--- Ubuntu 20.04.1 server, installed with IRCU and GNUWORLD. ---
Follow https://github.com/GNUWorldChannel/Installation-guide
to add cservice-web running too. 

ssh port: 22 Destination ip: check your DHCP and if you want
a static one, go /etc/netplan and look the file "static-readme".

NOTE: The first boot could take a while when the OS is
getting your ethernet adapter configuration.
We tested the network configuration, let it as bridge
do not change it to NAT, so please don´t. 
Always check ethernet adapter name there.

------------------------------------------
Users created: 


sudo user: anaconda

password: vaiacondios


user: root

password: vaiacondios


(where is ircd / gnuworld)

user: gnuworld

password: vaiacondios

------------------------------------------
What do you need to edit: 
ircd.conf
GNUWorld.conf 
cservice.conf
ccontrol.conf

You can start ircd + gnuworld using
./runall.sh file located at home in
gnuworld user :)

X login has "admin" as 1000 and the password
is temPass as usual.

If you want a custom 1000, then add it into the db
using the script as user id 2. 

------------------------------------------
Bugs?: You will tell us :)

If you have any question please read our guide since
we installed all from it.

https://github.com/GNUWorldChannel/Installation-guide

-Review- y2k/ARI3L
