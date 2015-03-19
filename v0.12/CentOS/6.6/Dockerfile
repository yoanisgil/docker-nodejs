FROM centos:centos6

MAINTAINER Yoanis Gil <gil.yoanis@gmail.com>

RUN yum -y groupinstall "Development tools"
RUN yum install -y tar wget
WORKDIR /tmp/
RUN wget http://nodejs.org/dist/v0.12.0/node-v0.12.0.tar.gz 2>/dev/null
RUN tar -xf node-v0.12.0.tar.gz
WORKDIR /tmp/node-v0.12.0 
RUN ./configure && make && make install
RUN rm -rf /tmp/node*
RUN yum remove -y autoconf automake bison byacc cscope ctags diffstat doxygen systemtap swig  subversion rpm-build redhat-rpm-config rcs patchutils patch libtool intltool  indent  gcc-gfortran  gcc-c++  flex elfutils
RUN yum clean all

CMD [ "node" ]
