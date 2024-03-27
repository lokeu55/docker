FROM rockylinux:9

# RUN yum -y update && yum -y install vsftpd && yum clean all
RUN yum -y install vsftpd && yum clean all

COPY vsftpd.conf.rockylinux9.template /etc/vsftpd/vsftpd.conf

VOLUME ["/var/ftp/pub"]
COPY WelcomToMyFTPSerer.txt /var/ftp/pub/WelcomToMyFTPSerer.txt

EXPOSE 21 20

CMD ["/usr/sbin/vsftpd"]
