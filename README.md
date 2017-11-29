# GoDaddy_Linux_DDNS
Simple script to check and update a Godaddy domain with your public ip address from you internet provider
Supported A and AAAA record

Reference by GoDaddy_Powershell_DDNS

You will need a GoDaddy developer account.
Go to GoDaddy developer site to create a developer account and get your key and secret

https://developer.godaddy.com/getstarted


Simple for Crontab
#minute hour    mday    month   wday    command
#*/15    *       *       *       *       /usr/local/bin/updategodaddy.sh www mydomain.com >> /var/log/updatedomain.log
