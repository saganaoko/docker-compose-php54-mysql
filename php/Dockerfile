FROM centos:centos7
RUN yum install -y php php-mcrypt php-mbstring
RUN yum -y install httpd; yum clean all; systemctl enable httpd.service
EXPOSE 80
COPY conf.d/* /etc/httpd/conf.d/
CMD ["/usr/sbin/init"]