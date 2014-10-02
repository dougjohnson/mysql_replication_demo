FROM centos:centos6

RUN yum -y install mysql-server 

RUN mysql_install_db

ADD mysql.cnf /etc/mysql/conf.d/mysql.cnf

ADD start /usr/bin/start-mysql

RUN chmod +x /usr/bin/start-mysql

EXPOSE 3306

# Start mysql server
CMD ["/usr/bin/start-mysql"]
