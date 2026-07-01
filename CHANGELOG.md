# Changelog

The **Next** series continues development of the plugins by the original author and focuses on ongoing maintenance, reliability improvements, and compatibility with current Unraid releases.

Development of the plugins will continue with ongoing maintenance, reliability improvements, and enhancements.

## Unassigned Devices - Next

## 2026.07.01

### Reliability & Device Management

- This release focuses on improving device handling, automation, and overall reliability. Numerous refinements were made to hotplug, detach, standby, ownership, and device script execution to make device management more predictable, especially in automated workflows.

### Automation & Scripting

- Device scripts have been significantly enhanced with isolated per-execution environments, preventing variable leakage between concurrent scripts while maintaining existing execution safeguards. New automation support also makes it easier to perform temporary hotplug operations that automatically clean up by unmounting devices when processing is complete.

### Diagnostics & Troubleshooting

- Diagnostics have been expanded with additional CIFS logging for remote share troubleshooting and log viewing for Historical Devices, making it easier to investigate detach, removal, and remote connectivity issues.

### Compatibility

- A small compatibility change removes the unused `LUKS` environment variable from the device script. Users with custom scripts referencing this variable should update those scripts accordingly.

## Unassigned Devices Plus - Next

### Maintenance

- This release updates several bundled system packages to their latest supported versions, providing ongoing compatibility, stability, and maintenance improvements.

## Unassigned Devices Preclear - Next

### Performance & Stability

- This release improves Preclear performance and reliability through internal refactoring and more efficient status handling. Signature verification has been strengthened, startup/shutdown edge cases have been resolved, and preclear operations now run with lower CPU and I/O priority to minimize impact on normal system workloads. The bundled `tmux` package has also been updated.

## Unassigned Devices - Next / Unassigned Devices Preclear - Next

## 2026.06.22

### Reliability & Stability

- Improved overall reliability of device management, hotplug handling, and background processing.
- Fixed several edge cases that could lead to stale device information or inconsistent status reporting.
- Improved synchronization between Unassigned Devices and Unassigned Devices Preclear during device events.
- Enhanced validation and execution checks to improve operational reliability.

### Performance & Efficiency

- Reduced unnecessary file operations and locking activity during configuration updates.
- Optimized disk status processing to reduce overhead and improve responsiveness.
- Streamlined internal status monitoring and update handling.

### Device & Share Management

- Improved handling of device information updates during hotplug events.
- Restored proper synchronization of Unassigned Devices shares when Unraid share services are refreshed.
- Improved overall consistency of device and share state management.

### Maintenance

- Corrected several PHP issues that could occur during array start and stop operations.
- Refactored portions of the disk status and validation logic for improved maintainability and long-term reliability.
- Improved validation routines used by Unassigned Devices Preclear.

## Unassigned Devices - Next

## 2026.06.19

### Reliability & Stability

- Improved overall mount, unmount, and device management reliability through significant internal refactoring.
- Added additional safeguards to prevent devices from entering invalid or improperly unmounted states.
- Improved shutdown handling to ensure devices and remote shares are cleanly unmounted and to reduce the chance of shutdown delays or hangs.
- Enhanced file locking and state management for more reliable configuration and status updates.

### Device Management

- Fixed several issues involving device removal, historical device handling, disk renaming, UUID changes, and mount point management.
- Added validation to ensure mount points are safe before mounting devices, helping prevent accidental data writes to incorrect locations.
- Improved handling of hotplug, formatting, and device-clearing events to keep device information synchronized and up to date.
- Fixed a long-standing issue where newly formatted NVMe partitions were not immediately recognized.

### Scripts & Automation

- Reworked device script execution, monitoring, logging, and abort handling for improved reliability.
- Added verification that scripts properly stop when aborted by the user or during system shutdown.
- Removed the legacy background script execution setting and simplified script behavior.
- Improved script logging and cleanup throughout the user interface.

### Performance & Responsiveness

- Improved UI refresh timing and responsiveness.
- Optimized hotplug processing by moving device assignment updates to background operations when appropriate.
- Reduced shutdown time by processing disk and remote share unmount operations in parallel.

### User Experience

- Improved warnings and messaging for device removal operations.
- Added additional logging and status reporting to help identify mount, unmount, and device-management issues.
- Cleaned up several dialogs and configuration workflows for a more consistent experience.

### Notes

- User Script abort operations involving rsync are limited by the way rsync spawns child processes. A pull request has been submitted to User Scripts to improve handling of these scenarios.

## 2026.05.26

### Improvements
- Updated encrypted disk handling to consistently use the built-in open and close operations
- Improved ZFS validation when formatting and mounting ZFS disks
- Updated help text and operation guidance for current functionality

### Fixes
- Extended VFAT sync timeout to improve reliability when unmounting devices outside of server shutdown
- Fixed encrypted disks failing to open during file system checks
- Fixed ntfs3 driver enablement on NTFS-formatted zvol devices
- Added validation to prevent use of reserved ZFS pool names

## 2026.05.10

### Fixes
- Fixed PHP warnings related to `htmlspecialchars()` on the main page

## 2026.04.22

### Stability and Reliability Improvements

- Improved script detection and termination for more accurate tracking and cleanup on UD devices.
- Fixed NTFS3 driver usage for encrypted NTFS disks and improved BTRFS usage reporting.
- Internal refactoring enhances reliability, reduces edge-case issues, and improves maintainability.

## 2026.04.06

### Major Improvements
- Improved overall reliability and stability of script execution, device monitoring, and runtime behavior  
- Enhanced locking mechanisms to prevent concurrency issues and potential deadlocks  
- Optimized page refresh behavior to reduce unnecessary activity and improve responsiveness  

### Remote Share Improvements
- Improved handling and reliability of remote share script execution  

### Filesystem and Device Enhancements
- Resolved issues with device statistics collection that could lead to stalled updates  
- Improved coordination of background processes to ensure proper execution order  

### User Interface Improvements
- Improved page refresh timing for better responsiveness and reduced system load  
- Prevented unnecessary device polling when the UI is not active  

### Diagnostics and Troubleshooting
- Improved error handling through proper return code propagation in command execution  
- Added safeguards such as timeouts to prevent indefinite hangs during background operations  

### Notes
- Improved compatibility with newer Unraid versions, including 7.3  
- Detailed technical changes are documented in the GitHub release notes

## 2026.03.27

Initial release of the **Next** series maintained by the original author.

The focus of this release is reliability, stability, and improved operational behavior...

Additional work has been done to reduce unnecessary polling and page refresh activity, UI changes to support Unraid 7.x Responsive Design, improve error handling, and add improved diagnostics and troubleshooting tools to assist with identifying configuration and mount issues.

### Major Improvements
- Significant reliability and stability improvements across device management, mounting, and monitoring
- Refactored device state handling and file locking for improved robustness
- Reduced unnecessary polling and UI refresh activity for better performance
- Improved handling of hotplug devices and device detection

### Remote Share Improvements
- Improved reliability of SMB and NFS remote share mounting
- Updated CIFS mount parameters to improve compatibility and prevent mount errors
- Added IPv6 support for SMB remote shares
- Improved diagnostics and testing tools for remote server connectivity

### Filesystem and Device Enhancements
- Improved support for encrypted disks and LUKS configuration options
- Improved handling of ZFS, Btrfs, ext4, and NTFS formatting and mounting
- Improved disk space calculations and mount status handling
- Added support for formatting disks compatible with the Unraid array

### User Interface Improvements
- Updated UI for compatibility with Unraid 7.x responsive design
- Reworked several settings pages for improved usability and clarity
- Improved tooltip behavior and UI layout consistency

### Diagnostics and Troubleshooting
- Added troubleshooting tools and diagnostics to assist with identifying configuration and mount issues
- Improved logging and debugging controls to reduce unnecessary log noise
- Added improved status reporting for device operations and preclear activity

### Notes
- Minimum supported Unraid version is now **6.12**
- This release resumes active development of the plugin
- Detailed technical changes are documented in the GitHub release notes

## Unassigned Devices Plus - Next

## 2026.03.27

Initial release of the **Next** series maintained by the original author.

### Fixes
- Updated filesystem tooling for compatibility with newer Unraid versions
- Replaced `exfat-utils` and `fuse-exfat` packages with `exfatprogs` when running Unraid 7.2
- Adjusted exFAT support for compatibility with Unraid 6.12 and 7.x
- Prevent removal of the `parted` package, which is now included and required by Unraid 7

### Notes
- Minimum supported Unraid version is now **6.12**
- This release resumes active development of the plugin
- Detailed technical changes are documented in the GitHub release notes

## Unassigned Devices Preclear - Next

## 2026.03.27

Initial release of the **Next** series maintained by the original author.

The focus of this release is reliability, stability, and improved operational behavior...

Additional work has been done for preclear robustness and UI changes to support Unraid 7.x Responsive Design.

### Improvements
- Refactored disk read/write routines for improved speed, reliability, and maintainability
- Improved pause and resume handling during preclear operations
- Added additional disk safety checks during preclear operations

### Enhancements
- Added periodic SMART monitoring during write operations to detect disk failures early
- Ensured all disk operations terminate immediately if a disk failure is detected
- Updated UI layout and dialog styling (Black Theme) for compatibility with recent Unraid UI changes
- Updated package handling and plugin structure

### Fixes
- Corrected several UI layout issues and tooltip behavior
- Fixed preclear icon visibility in Unassigned Devices page
- Corrected typo in preclear script

### Notes
- Minimum supported Unraid version is now **6.12**
- This release resumes active development of the plugin
- Detailed technical changes are documented in the GitHub release notes
