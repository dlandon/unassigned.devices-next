# Unassigned Devices – Next

The Unassigned Devices (Next) suite provides advanced management of unassigned drives and remote shares in Unraid, including:

- **Unassigned Devices**  
- **Unassigned Devices Plus**  
- **Unassigned Devices Preclear**

**Remote CIFS / NFS Mount Expectations**

Remote CIFS and NFS mounts are entirely dependent on network reliability.
Any LAN interruption, DNS delay, VPN blip, router restart, or WAN packet loss can cause mounts to stall or disconnect.

Internet-based mounts are inherently fragile.
Latency, NAT timeouts, firewall rules, ISP interruptions, and asymmetric routing all affect mount stability.

Once a mount is established, behavior is largely controlled by:
- Linux kernel
- CIFS/NFS protocol semantics
- Mount options (soft/hard, timeouts, retries)
- Remote server availability

Unassigned Devices can detect, mount, retry, and report remote mounts.
It cannot prevent disconnects caused by network or remote endpoint failures.

If a remote share drops offline, the cause is almost always the network or remote system — not the plugin.

These plugins are **independent alternatives** to the official Unraid plugins and offer enhanced mounting, formatting, and preclear capabilities while maintaining system stability.

This project continues the plugins authored by **dlandon** with enhancements and bug fixes.

Development in this repository begins from the codebase authored by **dlandon** and continues privately as of **March 2025**.

All development and commits dated **March 2025** and later are licensed under the custom license included in this repository.

- **No code in this repository is proprietary to Unraid or Limetech.**
- **All development and commits dated March 2025 and later are licensed under the custom license included in this repository.**

For support, discussions, and announcements, please use the **Discussions** tab in this repository.

# Installing Unassigned Devices

To install this plugin manually, enter either of the URLs below in the Enter URL field of the Plugins page.  The URL below will either install the latest or a specific version you choose.

Latest version: https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-next.plg

Specific version: https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-next.plg

Enter the release date "YYYY.MM.DD" of the specific version you want to install.  Be sure to keep the "v" before the release date.

# Installing Unassigned Devices Plus

To install this plugin manually, enter either of the URLs below in the Enter URL field of the Plugins page.  The URL below will either install the latest or a specific version you choose.

Latest version: https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-plus-next.plg

Specific version: https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-plus-next.plg

Enter the release date "YYYY.MM.DD" of the specific version you want to install.  Be sure to keep the "v" before the release date.

# Installing Unassigned Devices Preclear

To install this plugin manually, enter either of the URLs below in the Enter URL field of the Plugins page.  The URL below will either install the latest or a specific version you choose.

Latest version: https://raw.githubusercontent.com/dlandon/unassigned.devices-next/master/unassigned.devices-preclear-next.plg

Specific version: https://raw.githubusercontent.com/dlandon/unassigned.devices-next/vYYYY.MM.DD/unassigned.devices-preclear-next.plg

Enter the release date "YYYY.MM.DD" of the specific version you want to install.  Be sure to keep the "v" before the release date.
