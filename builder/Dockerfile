FROM ubuntu:18.04

RUN apt-get -qq update && \
    apt-get -qq -y install default-jdk && \
    apt-get -qq -y install maven && \
    apt-get -qq -y install git && \
    apt-get -qq -y install mc && \
    mkdir /data && \
    cd /data && \
    git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git && \
    cd /data/boxfuse-sample-java-war-hello && \
    mvn package

CMD [ "sh", "-c"]