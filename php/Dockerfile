FROM centos:centos7
RUN yum install -y epel-release unzip
RUN yum install -y php php-mcrypt php-mbstring php-pdo php-xml
RUN yum -y install httpd; yum clean all; systemctl enable httpd.service
EXPOSE 80
COPY conf.d/* /etc/httpd/conf.d/
COPY php.ini /etc/php.ini
COPY composer /usr/local/bin/
RUN chmod a+x /usr/local/bin/composer
CMD ["/usr/sbin/init"]