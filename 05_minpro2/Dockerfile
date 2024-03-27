FROM centos:7

RUN yum install -y httpd php && yum clean all

VOLUME ["/var/www.html", "/var/log/httpd"]
ADD src.tar /var/www/html

EXPOSE 80/tcp

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
