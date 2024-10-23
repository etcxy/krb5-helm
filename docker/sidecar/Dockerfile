FROM centos:7.5.1804

RUN curl -o /etc/yum.repos.d/CentOS-Base.repo https://mirrors.aliyun.com/repo/Centos-7.repo \
&& yum install -y krb5-workstation && \
    mkdir /krb5 && chmod 755 /krb5 

VOLUME ["/krb5","/dev/shm","/etc/krb5.conf.d"]

# USER 1001

ENTRYPOINT ["/rekinit.sh"]

