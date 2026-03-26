# Unassigned Devices - Next
Original author and continued development: Dan Landon

Included Plugins
- **Unassigned Devices**
- **Unassigned Devices Plus**
- **Unassigned Devices Preclear**

This plugin suite provides advanced disk management, remote mount handling, formatting utilities, and preclear capabilities for Unraid systems.

## Remote CIFS / NFS Mount Behavior

Remote CIFS and NFS mounts depend entirely on network and remote system stability.

LAN interruptions, DNS delays, VPN changes, router restarts, WAN latency, NAT timeouts, firewall rules, and remote server availability can all affect mount behavior.

## Once established, mount behavior is governed primarily by:
- **Linux kernel handling**
- **CIFS/NFS protocol semantics**
- **Mount options (soft/hard, timeouts, retries)**
- **Remote server responsiveness**

## Unassigned Devices can:
- **Detect and mount remote shares**
- **Retry failed connections**
- **Monitor and report mount status**

**It cannot prevent disconnects caused by network instability or remote endpoint failures.**

## About This Project

The Next series of this plugin is actively maintained by the original author and continues development of the project with ongoing fixes, improvements, and enhancements.

## Installing Unassigned Devices - Next

Enter one of the URLs below in the **Enter URL** field on the Unraid Plugins page.

### Latest version:

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-next.plg

### Specific version:

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-next.plg

Replace YYYY.MM.DD with the release date of the version you wish to install. Include the leading v in the URL.

## Installing Unassigned Devices Plus - Next

Enter one of the URLs below in the **Enter URL** field on the Unraid Plugins page.

### Latest version:

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-plus-next.plg

### Specific version:

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-plus-next.plg

Replace YYYY.MM.DD with the release date of the version you wish to install. Include the leading v in the URL.

## Installing Unassigned Devices Preclear - Next

Enter one of the URLs below in the **Enter URL** field on the Unraid Plugins page.

### Latest version:

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-preclear-next.plg

### Specific version:

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-preclear-next.plg

Replace YYYY.MM.DD with the release date of the version you wish to install. Include the leading v in the URL.

**Note:** The URL must begin with `https://raw.githubusercontent.com/`. GitHub page URLs (`github.com/.../blob/...`) will not install correctly.

For support, feature requests, and discussions, please use the Discussions tab.

## Distribution

This repository is the official distribution location for this plugin.

Users should install the plugin directly from the URLs provided in this repository to ensure they receive authentic and up-to-date releases.

Redistribution of this software through third-party repositories, plugin catalogs, mirrors, or repackaged installers is not authorized unless explicitly approved in writing by the author.

## License

This repository is maintained by the original author of the plugin.

Versions of this software publicly released prior to **March 18, 2025** remain licensed under the GNU General Public License (GPL) in accordance with their original terms.

Versions released as Next after that date are governed by the plugin-specific license included in the `LICENSE.md` file in this repository.

Users may install and use this software in accordance with the terms of that license.

## Support Development

If this plugin has been useful to you and you'd like to support ongoing development, you can optionally make a donation:

[Donate via PayPal](https://www.paypal.com/us/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=EJGPC7B5CS66E)

Support is appreciated, but never expected.
