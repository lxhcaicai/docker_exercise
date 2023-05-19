FROM ubuntu:20.04

MAINTAINER lxhcaicai "qwq@qq.com"

ENV JDK_HOME jdk1.8.0_131

ENV JDK_8 ./jdk-8u131-linux-x64.tar.gz

ENV MYPATH /usr/local

WORKDIR $MYPATH

RUN mkdir /usr/local/java

ADD $JDK_8 /usr/local/java/

ENV JAVA_HOME=/usr/local/java/$JDK_HOME/

ENV JRE_HOME $JAVA_HOME/jre

ENV CLASSPATH $JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar:$JRE_HOME/lib:$CLASSPATH

ENV PATH $JAVA_HOME/bin:$PATH

EXPOSE 80

CMD echo $MYPATHc

CMD echo "success---------ok"

CMD /bin/bash