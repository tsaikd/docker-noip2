FROM ubuntu:14.04

MAINTAINER tsaikd <tsaikd@gmail.com>

RUN apt-get update
RUN apt-get -y install wget gcc make
ADD docker_cmd_install.sh /install.sh
RUN mkdir -p /noip2
RUN wget http://www.noip.com/client/linux/noip-duc-linux.tar.gz -qO - | tar -C /noip2 --strip-components=1 -xzf -
RUN make -C /noip2 noip2

ENTRYPOINT ["/install.sh"]

