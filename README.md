# Security Testing
## How to install WebGoat + WebScarab
WebGoat works with Tomacat 7 and java, you have to download all the material from the `WebGoat` folder and install the software as following
```
$ sudo apt update
$ sudo apt install -y openjdk-8-jre
$ git clone git://github.com/filippodp/security.testing
$ mv security.testing/WebGoat/* . && rm security.testing/
$ tar -xvf apache-tomcat-7.0.82.tar.gz
$ mv WebGoat-5.4.war apache-tomcat-7.0.82/webapps/WebGoat.war
$ mv tomcat-users.xml apache-tomcat-7.0.82/config/tomcat-users.xml
$ rm apache-tomcat-7.0.82.tar.gz
```
Now we have all setup, start tomcat using `catalina.sh`
```
$ sh apache-tomcat-7.0.82/bin/catalina.sh start
```
WebGoat is located at `localhost:8080/WebGoat/attack`, the user and pswd are `guest` and `guest`. Enjoy haking!

WebScarab is more easy to install, just download it from the `WebScarab` folder (of course the file is `webscarab-20070504-1631.jar`) and run it with `java` command
```
$ git clone git://github.com/filippodp/security.testing
$ mv security.testing/WebScarab/* . && rm security.testing/

$ java -jar webscarab-20070504-1631.jar
```
## How to install SchoolMate
First of all we have to install the required software
```
$ apt update && apt upgrade
$ add-apt-repository ppa:ondrej/php
$ apt update
# set the password for mysql to root
$ apt install -y apache2 mysql-server /
                 php5.6 libapache2-mod-php5.6 php5.6-curl /
                 php5.6-gd php5.6-mbstring php5.6-mcrypt /
                 php5.6-mysql php5.6-xml php5.6-xmlrpc
$ git clone git://github.com/filippodp/security.testing
$ mv security.testing/SchoolMate/* . && rm security.testing/                 
$ tar -xvf SchoolMate.tar.gz -C /var/www/html
$ cd /var/www/html
```
Lauch `mysql` form terminal and execute
```
> mysql -u root -p
> source SchoolMate.sql;
> create user 'schoolmate'@'localhost' identified by 'schoolmate';
> grant all on schoolmate.* to 'schoolmate'@'localhost';
> flush privileges;
> source PopulateTables.sql;
> exit
```

## How to install/use JWebUnit
to do

##
<img src="https://github.com/filippodp/security.testing/blob/master/images/webgoat_logo.png" alt="WebGoat" height="70"><img src="https://github.com/filippodp/security.testing/blob/master/images/webscarab_logo.png" alt="WebScarab" height="70"><img src="https://github.com/filippodp/security.testing/blob/master/images/schoolmate_logo.gif" alt="SchoolMate" height="70"><img src="https://github.com/filippodp/security.testing/blob/master/images/jwebunit_logo.png" alt="JWebUnit" height="70">
