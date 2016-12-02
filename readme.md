
wget https://raw.githubusercontent.com/arsanto/backupdb/master/backupdb.sh && chmod +x backupdb.sh && cp backupdb.sh /usr/local/bin

############
#ganti password 

nano  /usr/local/bin/backupdb.sh

sehari sekali settiap jam 1 malam 

nano /etc/crontab

#############


0 1 * * * /usr/local/bin/backupdb.sh


###############




service crond restart
