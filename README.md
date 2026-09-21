# XG for Unraid Community Applications

This repository contains the Unraid Community Applications metadata for
[XG / XDCC Grabscher](https://github.com/CaptainEpix/xdcc-grabscher).

XG is a web-based IRC/XDCC download manager. This template installs the
maintained Mono/Docker compatibility fork published through GitHub Container
Registry.

## Container image

`ghcr.io/captainepix/xdcc-grabscher:latest`

## Template configuration

- **WebUI:** container port `5556`
- **Appdata:** `/config`
- **Downloads:** `/config/.config/XG/dl`

IRC servers, channels, NickServ credentials, and XG application settings are
configured through the XG WebUI.

## Project links

- Source: https://github.com/CaptainEpix/xdcc-grabscher
- Issues: https://github.com/CaptainEpix/xdcc-grabscher/issues
- Container: https://github.com/CaptainEpix/xdcc-grabscher/pkgs/container/xdcc-grabscher

## Licensing

The XG application is distributed under GPLv2.

The Community Applications template metadata in this repository is distributed
under the MIT License.
