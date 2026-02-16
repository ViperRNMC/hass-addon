# Home Assistant Add-ons

![Project Stage][project-stage-shield]
![Maintenance][maintenance-shield]


## About

My Home Assistant repository provides you a way to add additional capabilites
to your Home Assistant installation by adding add-ons that provide additional
functionality.

This is only 1 such example of a Home Assistant repository and there are many
others including the [Home Assistant Community Add-ons][repositoryCommunity] project.

## Installation

This add-on isn't included in Home Assistant by default and needs to be added from a GitHub repository. Don't worry - the process isn't too hard!

1. Within Home Assistant, navigate to **Configuration** > ** Add-ons, Backups & Supervisor** 
1. Click **ADD-ON STORE** > **Menu** (3 dot elipsis, top right) > **Repositories**
1. Add the following Repository

```txt
https://github.com/ViperRNMC/hass-addon
```

## Add-ons provided by this repository

### &#10003; [InfluxDB2][influxdb2-addon]

![Supports amd64 Architecture][influxdb2-amd64-shield]
![Supports aarch64 Architecture][influxdb2-aarch64-shield]
![Local Build][influxdb2-local-build]

InfluxDB is an open source time series database optimized for high-write-volume.
It's useful for recording metrics, sensor data, events, and performing analytics.

Details (from `influxdb2/config.json`):

- **Version:** 2025.8.0
- **Supported architectures:** aarch64, amd64
- **Home Assistant requirement:** 2024.2.0
- **Startup:** services
- **Ports:** 8086/tcp -> 8086
- **Options:** reporting, ssl, certfile, keyfile, envvars
- **Docs:** [:books: InfluxDB2 add-on documentation][influxdb2-doc]

### &#10003; [Rinkhals Timelapse][rinkhals-addon]

Rinkhals Timelapse creates timelapse videos from snapshots produced by
Rinkhals-enabled printers or cameras. Configure and enable the add-on via
the Home Assistant add-on store after adding this repository.

Details (from `rinkhals-timelapse/config.json`):

- **Version:** 1.0.0
- **Supported architectures:** amd64, armv7, armhf, aarch64
- **Startup:** services
- **Ingress:** yes
- **Maps:** config:rw, media:rw
- **Options:** printer_ip (str), media_path (str)



[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2026.svg
[influxdbv1]: https://github.com/hassio-addons/addon-influxdb
[repositoryCommunity]: https://github.com/hassio-addons/repository

[comment]: <> (-- INFLUXDB2 --)
[influxdb2-local-build]: https://img.shields.io/badge/Home%20Assistant%20--%20local%20build-YES-orange.svg
[influxdb2-ingressSupport]: https://img.shields.io/badge/Home%20Assistant%20--%20ingress%20support-NO-red
[influxdb2-aarch64-shield]: https://img.shields.io/badge/aarch64-untested-orange.svg
[influxdb2-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[influxdb2-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[influxdb2-armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[influxdb2-i386-shield]: https://img.shields.io/badge/i386-no-red.svg

[influxdb2-doc]: https://github.com/ViperRNMC/hass-addon/blob/main/influxdb2/DOCS.md

[influxdb2-addon]: https://github.com/ViperRNMC/hass-addon/blob/main/influxdb2

