FROM debian:wheezy
MAINTAINER MeteorHacks Pvt Ltd.

ENV METEORD_DIR /opt/meteord
COPY scripts $METEORD_DIR

RUN bash $METEORD_DIR/init.sh

RUN sudo apt-get install libstdc++6

EXPOSE 80
ENTRYPOINT bash $METEORD_DIR/run_app.sh
