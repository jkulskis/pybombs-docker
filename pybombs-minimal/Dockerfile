FROM ubuntu:18.04
# originally from https://github.com/gnuradio/pybombs-docker

ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update
# Install python3 and python2.7 since gnuradio 3.7 uses python2
RUN apt-get install -y --no-install-recommends python3.6 python3-pip python3-apt apt-utils
RUN apt-get install -y --no-install-recommends python2.7 python-pip
RUN pip3 install --upgrade pip
RUN pip3 install pybombs
RUN pybombs auto-config
RUN pybombs config makewidth 2