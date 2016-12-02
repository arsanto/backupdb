
wget https://raw.githubusercontent.com/arsanto/backupdb/master/backupdb.sh && chmod +x backupdb.sh && cp backupdb.sh /usr/local/bin

############
#ganti password 

nano  /usr/local/bin/backupdb.sh

seminngu sekali 

nano /etc/crontab

#############


0 0 * * 1 /usr/local/bin/backupdb.sh


###############



service cron restart
service crond restart
