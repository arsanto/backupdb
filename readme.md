
wget https://raw.githubusercontent.com/arsanto/backupdb/master/backupdb.sh && chmod +x backupdb.sh && cp backupdb.sh /usr/local/bin

############
#ganti password 

nano  /usr/local/bin/backupdb.sh

Next thing is to set up a simple cronjob to schedule a backup every night at 1 am:

nano /etc/crontab

#############


0 1 * * * root /usr/local/bin/backupdb.sh


###############



service cron restart
service crond restart
