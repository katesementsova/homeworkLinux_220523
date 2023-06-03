# homeworkLinux_220523

[ec2-user@ip-172-31-33-20 ~]$ cd /opt
[ec2-user@ip-172-31-33-20 opt]$ cd 040423_evening/
[ec2-user@ip-172-31-33-20 040423_evening]$ cd sementsova/
[ec2-user@ip-172-31-33-20 sementsova]$ nano taskSEMENTSOVA.sh


#!/bin/bash

tdate=$(date +"%H%M%S")

for run in {1..10}
do
number=$run
file="${number}_${tdate}"
touch $file
done

Ctrl X

[ec2-user@ip-172-31-33-20 sementsova]$ crontab -e
crontab: installing new crontab

[ec2-user@ip-172-31-33-20 sementsova]$ crontab -l
#* * * * * /opt/280323_morning/SergejsPonomarenko/script555.sh >> /opt/280323_morning/SergejsPonomarenko/output1.txt
#* * * * * /opt/280323_morning/zakorko/script555.sh >> /opt/280323_morning/zakorko/output.txt
#* * * * * /opt/280323_morning/Viktar_Chumachenka/script555.sh >> /opt/280323_morning/Viktar_Chumachenka/output.txt
15 * * * * /opt/280323_morning/ikar-zindo/taskIVAN.sh
#* * * * * /opt/280323_morning/Lenok/script555.sh >> /opt/280323_morning/Lenok/output.txt
15 * * * * /opt/280323_morning/sukhikh/tasksukhikh.sh
15 * * * * /opt/o4o423_evening/sementsova/taskKATYA.sh
