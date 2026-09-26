# XG for Unraid Community Applications

This repository contains the Unraid Community Applications metadata for
[XG / XDCC Grabscher](https://github.com/CaptainEpix/xdcc-grabscher).

XG is a web-based IRC/XDCC download manager. This template installs the
maintained Mono/Docker compatibility fork published through GitHub Container
Registry.

## Container image

`ghcr.io/captainepix/xdcc-grabscher:latest`

Fixed versions are tagged like `3.3.3.0-mono2026`.

## Template configuration

- **WebUI:** container port `5556`
- **Appdata:** `/config`
- **Downloads:** `/config/.config/XG/dl`

IRC servers, channels, NickServ credentials, and XG application settings are
configured through the XG WebUI.

### Optional settings

| Setting | Variable | Purpose |
| --- | --- | --- |
| Category folders | `XG_CATEGORY_FOLDERS` | `all` or a list such as `tv,movies`: Sonarr/Radarr grabs go into a subfolder per category. |
| Passive DCC ports | `XG_PASSIVE_DCC_PORTS` | For example `50000-50004`: enables passive (reverse) DCC on these ports. |
| Passive DCC public IP | `XG_PASSIVE_DCC_IP` | Public IPv4 address; detected automatically when empty. |
| Silent bot timeout | `XG_COMPAT_SILENT_BOT_SECONDS` | Seconds before a Sonarr/Radarr grab fails when the bot never answers (default 900). |

For passive DCC, also fill in the *Passive DCC port* entries (shown under
*Show more settings*) with the same ports, and forward those ports on your
router to the Unraid server.

Prowlarr, Sonarr and Radarr setup is described in the
[XG README](https://github.com/CaptainEpix/xdcc-grabscher/blob/mono-2026/README.md#prowlarr--sonarr--radarr-integration).

## Project links

- Source: https://github.com/CaptainEpix/xdcc-grabscher
- Issues: https://github.com/CaptainEpix/xdcc-grabscher/issues
- Container: https://github.com/CaptainEpix/xdcc-grabscher/pkgs/container/xdcc-grabscher

## Licensing

The XG application is distributed under GPLv2.

The Community Applications template metadata in this repository is distributed
under the MIT License.
