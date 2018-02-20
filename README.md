# Security Testing
## How to install WebGoat + WebScarab
some text
```
$ some commands
$ install tomcat 7
$ install java
$ get WebGoat
& put it into the folder
```
some text
WebScarab is more easy, just download it from the WebScarab folder (of course the file is `webscarab-20070504-1631.jar`) and run it
```
$ java -jar webscarab-20070504-1631.jar
```
## How to install SchoolMate
First of all we have to install the required software
```
$ apt update && apt upgrade
$ add-apt-repository ppa:ondrej/php
$ apt update
$ apt install -y apache2 mysql-server php5.6 libapache2-mod-php5.6 php5.6-curl php5.6-gd php5.6-mbstring php5.6-mcrypt php5.6-mysql php5.6-xml php5.6-xmlrpc
$ wget -O SchoolMate.tar.gz https://netix.dl.sourceforge.net/project/schoolmate/SchoolMate/SchoolMate%20V1.5.4/SchoolMate_v1.5.4.tar.gz
tar -xvf SchoolMate.tar.gz -C /var/www/html

```





mysql -u root -p

source SchoolMate.sql;
create user 'schoolmate'@'localhost' identified by 'schoolmate';
grant all on schoolmate.* to 'schoolmate'@'localhost';
flush privileges;
insert into schoolmate.users (username,password) values ('Larry Stooge',md5('Larry Stooge'));


## How to install/use JWebUnit
to do
