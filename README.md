#!/bin/bash
# apache-web-server
creating bash script to install apache webserver
# Update package list and install Apache
sudo yum update -y
sudo yum install -y httpd
# Start Apache and enable it to start on boot
sudo systemctl start httpd
sudo systemctl enable httpd
# Restart Apache to ensure changes take effect
sudo systemctl restart httpd

