ARG BUILD_FROM
FROM $BUILD_FROM

LABEL Monyol <monyol@monyol.com>

# Set shell
SHELL ["/bin/bash", "-o", "pipefail", "-c"]

ENV LANG C.UTF-8

# Install requirements for add-on
RUN apk update && apk add --no-cache    \
#    avahi                               \
#    bash jq iw net-tools                \
#    sudo busybox-extras                 \
#    hostapd networkmanager iptables     \
    linux-firmware                      \
    linux-firmware-other                \
#    linux-firmware-ath6k                \
#    linux-firmware-ath10k               \
#    linux-firmware-ath9k_htc &&         \
#    rm -rf /var/cache/apk/*

COPY dvb-usb-dib0700-1.20.fw /lib/firmware/dvb-usb-dib0700-1.20.fw
#COPY udhcpd.conf /etc/udhcpd.conf
#COPY run.sh /
#RUN chmod a+x /run.sh

#CMD [ "/run.sh" ]
