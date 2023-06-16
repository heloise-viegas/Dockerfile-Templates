FROM ubuntu:22.04
RUN apt-get update -y && apt-get upgrade -y
RUN apt-get -y install wget
RUN wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1f-1ubuntu2.18_amd64.deb
RUN dpkg -i libssl1.1_1.1.1f-1ubuntu2.18_amd64.deb
RUN wget https://nginx.org/packages/ubuntu/pool/nginx/n/nginx/nginx_1.22.1-1~bionic_amd64.deb  
RUN dpkg -i nginx_1.22.1-1~bionic_amd64.deb
CMD ["nginx", "-v"]


#RUN apt-get update && \
 #   apt-get install -y -q curl gnupg2
#RUN curl http://nginx.org/keys/nginx_signing.key | apt-key add -

#RUN apt-get update && \
 #   apt-get install -y -q nginx

#ADD nginx.conf /etc/nginx/
#ADD server.conf /etc/nginx/conf.d

#EXPOSE 443 80

#CMD ["nginx", "-g", "daemon off;"]
