
wget https://raw.githubusercontent.com/arsanto/backupdb/master/install.sh && chmod +x install.sh
############
Next thing is to set up a simple cronjob to schedule a backup every night at 1 am:
nano /etc/crontab
#############
0 1 * * * root /usr/local/sbin/kinamo_mysqlbackup.sh


###############
service cron restart
service crond restart
