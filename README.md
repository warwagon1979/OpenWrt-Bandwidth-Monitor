# OpenWrt Bandwidth Dashboard

A lightweight bandwidth, DNS, alerting, and Smart Home dashboard for OpenWrt.

## Current version

**2.1.88**

## Highlights

- Per-device bandwidth monitoring and usage history
- Live bandwidth monitoring
- DNS / domain monitoring
- Optional tcpdump DNS capture for devices using external DNS servers
- Persistent DNS history with configurable retention
- Search saved DNS history across multiple days
- Calendar view that highlights days with matching DNS results
- Email alerts, including Minimum Usage by Time
- Automatic dashboard backups and restore
- Smart Home water, electricity, temperature, and humidity monitoring
- WireGuard peer information
- CPU and process monitoring
- Device naming, grouping, categories, and dashboard cards

## Minimum Usage by Time alerts

You can configure an alert for a specific device and require it to upload or download a minimum amount of data by a certain time.

Example:

> QuickBooks PC must upload at least 1 GB by 4:00 AM.

If the device has not reached the required amount by the deadline, the dashboard sends an email alert.

## DNS history

Recent DNS records can be kept temporarily in RAM or saved to the storage location selected during setup.

When persistent DNS storage is enabled, you can:

- Choose how many days of DNS history to retain
- Search across all retained DNS history
- See the date and time for matching records
- View matching days on a calendar
- Select a day to show only that day's results
- Browse all matching results in a continuously scrolling list
- Clear DNS history with confirmation

## Installation

Upload the current ZIP installer to your OpenWrt router, extract it under `/tmp`, make `install.sh` executable, and run it.

Example:

```sh
cd /tmp
unzip openwrt-bandwidth-dashboard-install-2.1.88.zip
cd openwrt-bandwidth-dashboard-install-2.1.88
chmod +x install.sh
./install.sh
```

## Ownership and contributions

This is the official project repository maintained by **warwagon1979**.

Anyone may view the repository and suggest changes, but only repository members with write access can directly modify this repository.
