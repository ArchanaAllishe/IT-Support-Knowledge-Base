# Network Troubleshooting Guide

## Purpose

This guide provides a structured approach for diagnosing and resolving common network connectivity issues in Windows environments. It covers wired and wireless connections, IP configuration, DNS resolution, and internet access using standard troubleshooting techniques.

![Network Troubleshooting Flowchart](images/network-troubleshooting-flowchart.png)
---

## Scope

This guide applies to:

* Windows 10
* Windows 11
* Wired (Ethernet) connections
* Wireless (Wi-Fi) connections
* Small office and enterprise networks

---

# Common Network Issues

Typical issues reported by users include:

* No internet connection
* Unable to connect to Wi-Fi
* Slow internet performance
* Limited or no network access
* Unable to access shared folders
* Unable to reach internal applications
* VPN connection problems
* Intermittent network connectivity

---

# Standard Troubleshooting Process

## Step 1 – Gather Information

Ask the user:

* What issue are you experiencing?
* When did the problem begin?
* Is the issue affecting one device or multiple devices?
* Are you using Wi-Fi or Ethernet?
* Can you access any websites?
* Have there been any recent changes?

---

## Step 2 – Verify Physical Connections

For Ethernet connections:

* Confirm the network cable is securely connected.
* Check for link lights on the network port.
* Test with another cable if available.

For Wi-Fi connections:

* Verify Wi-Fi is enabled.
* Confirm Airplane Mode is disabled.
* Ensure the correct wireless network (SSID) is selected.

## Example Network Topology

![Typical Network Topology](images/network-topology-example.png)

---

## Step 3 – Check Network Status

Verify:

* Connected network
* Signal strength
* Network adapter status
* IP address assignment
* Default gateway
* DNS server configuration

## Windows Network Settings

![Windows Network Settings](images/windows-network-settings.png)

---

## Step 4 – Test Connectivity

Perform connectivity tests in this order:

1. Ping the local computer.
2. Ping the default gateway.
3. Ping a public IP address (for example, `8.8.8.8`).
4. Ping a website by name (for example, `www.microsoft.com`).

This helps determine whether the issue is related to local networking, internet connectivity, or DNS resolution.

---

## Step 5 – Resolve the Issue

Possible solutions include:

* Restart the computer.
* Restart the router or wireless access point.
* Disable and re-enable the network adapter.
* Renew the IP address.
* Flush the DNS cache.
* Update the network adapter driver.
* Forget and reconnect to the Wi-Fi network.

---

# Common Windows Network Commands

| Command                    | Purpose                                |
| -------------------------- | -------------------------------------- |
| `ipconfig /all`            | Display detailed network configuration |
| `ipconfig /release`        | Release the current IP 

![IPConfig Example](images/ipconfig-example.png)

address         |
| `ipconfig /renew`          | Request a new IP address               |
| `ipconfig /flushdns`       | Clear the DNS resolver cache           |
| `ping`                     | Test network 
connectivity              |

![Ping Example](images/ping-example.png)

| `tracert`                  | Trace the path to a destination        |
| `nslookup`                 | Verify DNS name resolution             |
| `netsh wlan show profiles` | Display saved Wi-Fi profiles           |


---

# Common Issues and Resolutions

## No Internet Connection

### Possible Causes

* Router offline
* ISP outage
* Network adapter disabled
* Incorrect IP configuration

### Resolution

* Restart the router.
* Verify adapter status.
* Renew the IP address.
* Test internet connectivity.

---

## Connected to Wi-Fi but No Internet

### Possible Causes

* DNS issue
* Gateway unreachable
* ISP outage
* Captive portal authentication required

### Resolution

* Ping the default gateway.
* Ping a public IP address.
* Flush the DNS cache.
* Reconnect to the wireless network.

---

## Slow Network Performance

### Possible Causes

* Weak Wi-Fi signal
* Network congestion
* Background downloads
* Outdated network driver

### Resolution

* Move closer to the wireless access point.
* Restart networking equipment.
* Pause unnecessary downloads.
* Update network drivers.

---

## Unable to Access Shared Resources

### Possible Causes

* Incorrect permissions
* DNS resolution issues
* Network discovery disabled
* Firewall restrictions

### Resolution

* Verify permissions.
* Confirm hostname resolution.
* Enable Network Discovery if appropriate.
* Test access using the IP address.

---

# Basic Troubleshooting Checklist

* Verify physical connections.
* Confirm network adapter status.
* Check IP address assignment.
* Verify gateway and DNS settings.
* Test local connectivity.
* Test internet connectivity.
* Restart network equipment if necessary.
* Document findings and resolution.

---

# User Communication

### No Internet Connection

> I verified your network connection and identified the source of the issue. The connection has been restored, and I confirmed internet access is working normally. Please let me know if the issue returns.

### Wi-Fi Connection Issue

> Your wireless connection has been restored. If you experience additional connectivity problems, restarting the computer and reconnecting to the network is a good first step before contacting IT Support.

---

# Related Articles

* Cisco Wireless Basics
* DNS and DHCP
* Network Diagnostic Tools
* Windows Troubleshooting Guide
* ODBC SQL Server Connectivity
