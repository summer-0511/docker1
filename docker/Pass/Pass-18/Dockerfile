FROM upload-labs

MAINTAINER c0ny1 <root@gv7.me>
ENV LC_ALL C.UTF-8
ENV TZ=Asia/Shanghai

COPY . /tmp/

# install upload-labs/Pass
RUN cd /tmp/ &&\
    git clone https://github.com/summer-0511/docker1.git &&\
    rm -rf /var/www/html/Pass/* &&\
    mkdir /var/www/html/Pass/upload &&\
    mv /tmp/docker1/Pass/Pass-18/* /var/www/html/Pass/ &&\
    chown www-data:www-data -R /var/www/html/ && \
    rm -rf /tmp/*

EXPOSE 80