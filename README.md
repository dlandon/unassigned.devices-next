# Unassigned Devices – Next
Included Plugins

- **Unassigned Devices**
- **Unassigned Devices Plus**
- **Unassigned Devices Preclear**

This plugin suite provides advanced disk management, remote mount handling, formatting utilities, and preclear capabilities for Unraid systems.

### Remote CIFS / NFS Mount Behavior

Remote CIFS and NFS mounts depend entirely on network and remote system stability.

LAN interruptions, DNS delays, VPN changes, router restarts, WAN latency, NAT timeouts, firewall rules, and remote server availability can all affect mount behavior.

### Once established, mount behavior is governed primarily by:
- **Linux kernel handling**
- **CIFS/NFS protocol semantics**
- **Mount options (soft/hard, timeouts, retries)**
- **Remote server responsiveness**

### Unassigned Devices can:
- **Detect and mount remote shares**
- **Retry failed connections**
- **Monitor and report mount status**

**It cannot prevent disconnects caused by network instability or remote endpoint failures.**

### About This Project

This project continues development of the Unassigned Devices plugin suite originally authored by Dan Landon, with enhancements, stability improvements, and expanded functionality.

Development in this repository reflects ongoing work by the original author.

All versions publicly released under the GPL prior to February 17, 2025 remain licensed under the GPL.
Versions released after that date are governed by the custom license included in this repository.

For support, feature requests, and discussions, please use the Discussions tab.

### Installing Unassigned Devices (Next)

Enter one of the URLs below in the “Enter URL” field on the Unraid Plugins page.

Latest version:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-next.plg

Specific version:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-next.plg

Replace YYYY.MM.DD with the release date of the version you wish to install.
Include the leading v in the URL.

### Installing Unassigned Devices Plus (Next)

Latest version:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-plus-next.plg

Specific version:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-plus-next.plg

### Installing Unassigned Devices Preclear (Next)

Latest version:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-preclear-next.plg

Specific version:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-preclear-next.plg

### License Notice

This repository is maintained by the original author of the Unassigned Devices plugin suite.

Individual users may install and use this software in accordance with the license terms.

Versions released prior to February 17, 2025 remain licensed under the GPL.
Subsequent versions are licensed under the custom license included in this repository.
