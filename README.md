#!/bin/bash
yum update -y
yum install httpd -y
service httpd start
chkconfig httpd on
cd /var/www/html
echo "<html><h1>This is not a Magic. It is proof of hard work!</h1></html>"  >  index.html

