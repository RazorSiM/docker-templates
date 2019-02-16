# Raz unRaid Templates
Templates i made from docker containers i use

## Home Assistant Configurator

Template based on https://hub.docker.com/r/causticlab/hass-configurator-docker/

You can check the project's Github repo here: https://github.com/danielperna84/hass-configurator

To install, be sure to point the /hass-config volume to your home assistant docker container folder setting
ex: `/mnt/usr/cache/appdata/home-assistant`


After the installation, you can add the configurator to a panel iframe by editing the configuration.yaml:

    panel_iframe:
        configurator:
        title: Configurator
        icon: mdi:wrench
        url: http://123.123.132.132:3218

## Bitwarden

Bitwarden template for unraid, based on https://hub.docker.com/r/mprasil/bitwarden

To use it with chrome and its windows/mobile applications, you have to setup a reverse proxy by letsencrypt or Nginx Proxy Manager.

More informations can be found here: https://blog.linuxserver.io/2019/01/15/self-hosting-bitwarden/

## Yourls

Based on the official image: https://hub.docker.com/_/yourls/

You will need something like [Nginx Proxy Manager](https://forums.unraid.net/topic/76460-support-djoss-nginx-proxy-manager/) or Letsencrypt container to create a reverse proxy and use the yourls
