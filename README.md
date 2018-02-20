# Security Testing
## How to install WebGoat + WebScarab
WebGoat works with Tomacat 7 and java download all we need from the folder `WebGoat` and install them
```
$ sudo apt update
$ sudo apt install -y openjdk-8-jre
$ how to get folder
$ tar -xvf apache-tomcat-7.0.82.tar.gz
$ mv WebGoat-5.4.war apache-tomcat-7.0.82/webapps/WebGoat.war
$ mv tomcat-users.xml apache-tomcat-7.0.82/config/tomcat-users.xml
$ rm apache-tomcat-7.0.82.tar.gz
```
Now we have all setup, start tomcat using `catalina.sh`
```
$ sh apache-tomcat-7.0.82/bim/catalina.sh start
```
WebGoat is located at `localhost:8080/WebGoat/attack`, the uername and password are `guest` and `guest`. Enjoy haking!

WebScarab is more easy, just download it from the WebScarab folder (of course the file is `webscarab-20070504-1631.jar`) and run it
```
$ how to get the folder
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
