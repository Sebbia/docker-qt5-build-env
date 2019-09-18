FROM debian:9

RUN apt-get update && apt-get install -y wget

ENV QT_VERSION 5.12.1

WORKDIR /opt

RUN export QT_FOLDER=$(echo ${QT_VERSION} | sed -r 's/^([0-9]+\.[0-9]+)(\.[0-9]+)?$/\1/') && \
    wget https://download.qt.io/archive/qt/${QT_FOLDER}/${QT_VERSION}/qt-opensource-linux-x64-${QT_VERSION}.run