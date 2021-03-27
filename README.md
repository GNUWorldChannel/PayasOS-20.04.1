<p style="text-align:center;"><img src="https://github.com/GNUWorldChannel/PayasOS-20.04.1/blob/main/logo-final.png" alt="PayasOS 20.04.1 by y2k and ARI3L"></p>

# PayasOS-20.04.2 server WITH cservice-web. (03/2021)

Note: We added to the IPR these range: 192.168.1.0/24 - 192.168.100.0/24 - 10.0.0.0/24 - 127.0.0.0/24 
for the user Admin. So if you need to add another one like your public IPV4, do this:
nano ipr.sql 

Write your own ip. (200.200.200.0/24 is an example).

insert into ip_restrict (id, user_id, added_by, added, type, expiry, value) values (1, 1, 1, now()::abstime::int4, 1, 0, '200.200.200.0/24');

Save the file with (CTRL+O)

With the gnuworld running, perform:

gnuworld@ircd:~/gnuworld/cservice-web/php_includes$ /usr/local/pgsql/bin/psql -h 127.0.0.1 cservice < ipr.sql 

# PayasOS-20.04.2 server WITHOUT cservice-web (03/2021)

Request us access vía: 
https://drive.google.com/file/d/1rUz2mS0KX4teNJ_yevrpXa5OsqOxTrku/view?usp=sharing

For the cservice-web version: 
https://drive.google.com/file/d/1WX3pDHPGgz45NZTMdb6KFOjHcL0xoYjA/view?usp=sharing

This is a VM image created under Virtual Box, uncompress, edit mandatory
config files and enjoy :)

--- Ubuntu 20.04.2 server, installed with IRCU and GNUWORLD. ---
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
