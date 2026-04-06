# Changelog

The **Next** series continues development of the plugins by the original author and focuses on ongoing maintenance, reliability improvements, and compatibility with current Unraid releases.

Development of the plugins will continue with ongoing maintenance, reliability improvements, and enhancements.

## Unassigned Devices - Next

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
