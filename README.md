
# Security Testing
## How to install WebGoat
some text
```
$ some commands
```
some text

## How to install SchoolMate
First of all we have to install the required software
```
$ sudo apt update && apt upgrade
$ sudo add-apt-repository ppa:ondrej/php
$ sudo apt update
$ apt install -y apache2 mysql-server php5.6 libapache2-mod-php5.6 php5.6-curl php5.6-gd php5.6-mbstring php5.6-mcrypt php5.6-mysql php5.6-xml php5.6-xmlrpc
```





mysql -u root -p

source SchoolMate.sql;
create user 'schoolmate'@'localhost' identified by 'schoolmate';
grant all on schoolmate.* to 'schoolmate'@'localhost';
flush privileges;
insert into schoolmate.users (username,password) values ('Larry Stooge',md5('Larry Stooge'));


