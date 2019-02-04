# GoDaddy_Linux_DDNS
Simple script to check and update a Godaddy domain with your public ip address from you internet provider

Supported A and AAAA record

You will need a GoDaddy developer account.
Go to GoDaddy developer site to create a developer account and get your key and secret

https://developer.godaddy.com/getstarted


Sample for crontab

#*/15    *       *       *       *       /usr/local/bin/updategodaddy.sh AAAA www mydomain.com >> /var/log/updatedomain.log

Reference by GoDaddy_Powershell_DDNS

# Issues:

  1. -d provided data should be a json array, otherwise api errors out, so $request='[{"data":"1.1.1.1"}]'  
  2. usage: app $type $name $domain. the name has to be defined for this script to be executed successfully, otherwise it'll error out instead of giving out an information.
