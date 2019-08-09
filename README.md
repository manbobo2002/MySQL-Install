# MySQL-Install

# Before You Begin
su root  
#enter password  
yes | yum update  
yes | yum install wget  

# Install MySQL
wget http://repo.mysql.com/mysql-community-release-el7-5.noarch.rpm
sudo rpm -ivh mysql-community-release-el7-5.noarch.rpm  
yes | yum update  
yes | yum install mysql-server  
systemctl start mysqld  

# Harden MySQL ServerPermalink
mysql_secure_installation  

# Root Login
mysql -u root -p  
