# check_systemctl.sh
Nagios XI check for service check with systemctl command 
eg. 
command[Check Service apache2]=/usr/local/nagios/libexec/check_service.sh -t "systemctl status apache2" -u root
command[Check Service apache2]=/usr/local/nagios/libexec/check_service.sh -s apache2
command[Check Service apache2]=/usr/local/nagios/libexec/check_service.sh -t "systemctl status apache2" -u root -o linux



visudo 
#Nagios
nagios ALL=NOPASSWD: /usr/local/nagios/libexec/*
