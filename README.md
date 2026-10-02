# Nmap Network Scanning

## Objective

The objective of this project is to perform basic network reconnaissance using
Nmap against an authorized local machine/virtual machine. The scan identifies
open ports, running services, service versions, and the probable operating
system.

## What is Nmap?

Nmap (Network Mapper) is an open-source network scanning tool used to discover
hosts and services on a computer network. It can identify open ports, running
services, service versions, and operating-system information.

## Why Network Scanning Matters

Network scanning is an important part of cybersecurity because it helps identify
which services are exposed on a system. Administrators and security
professionals can use this information to:

- Identify unnecessary open ports
- Discover running network services
- Detect potentially outdated services
- Reduce the system's attack surface
- Improve firewall and network security

## Tools Used

- Nmap
- Linux/Kali Linux terminal
- Local/authorized target machine
- GitHub

## Nmap Installation

On Debian/Ubuntu/Kali Linux, Nmap can be installed with:

```bash
sudo apt update
sudo apt install nmap

## Scans Performed

### 1. Basic Scan

Command:

```bash
nmap 192.168.1.19

That is fine **if `192.168.1.19` is your own computer or a machine you have permission to scan**.

You can continue the README below it with something like:

```markdown
## Scan Results

The scan identified the following open ports:

- 135/tcp - MSRPC
- 139/tcp - NetBIOS-SSN
- 445/tcp - Microsoft-DS / SMB

The target was identified as Microsoft Windows 11.

## Security Observations

- Port 135 is associated with Microsoft RPC services.
- Port 139 is associated with NetBIOS Session Service.
- Port 445 is associated with SMB file and printer sharing.
- Unnecessary exposed services should be restricted using firewall rules.

## Ethical Use

Nmap scanning was performed only on an authorized/local system for educational purposes.

Nmap should only be used on systems that you own or have explicit permission to scan.
