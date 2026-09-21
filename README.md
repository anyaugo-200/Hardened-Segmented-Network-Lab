# Project 03 - Hardened Segmented Network Lab

## Overview

This project is a pfSense network segmentation lab showing how WEB, DB, and ADMIN zones can be separated, how lateral movement can be blocked, how firewall management can be restricted to an admin network, and how blocked events can be logged and monitored.

**Evidence report:** [project-03-hardened-segmented-network-lab.pdf](project-03-hardened-segmented-network-lab.pdf)

## Scope

- Target: Juice Shop hardened segmented network lab
- Environment: controlled local VirtualBox lab
- Firewall platform: pfSense
- Assessment type: network architecture, firewall policy, traffic validation, admin access hardening, logging, and monitoring
- Evidence: 42 screenshots across 9 project sections
- Classification: public portfolio sample / capability demonstration

## Lab Goals

- Build a segmented lab with WAN, WEB, DB, and ADMIN zones
- Assign interfaces, static gateway IPs, and DHCP scopes
- Implement firewall aliases and segmentation rules
- Allow required outbound traffic while blocking unwanted lateral movement
- Restrict pfSense management to the ADMIN network
- Capture firewall logs and monitoring evidence for blocked traffic

## Evidence Sections

| Test | Section | What was validated |
| --- | --- | --- |
| 01 | Firewall Installation and Baseline | pfSense identity, version, and healthy WAN/LAN baseline. |
| 02 | Network Architecture and Zones | VirtualBox adapter layout for WAN, WEB, DB, and ADMIN zones. |
| 03 | Interface Assignments and DHCP | Interface assignments, static gateway IPs, and DHCP scopes for segmented clients. |
| 04 | Firewall Rules and Segmentation Policy | Aliases and rules separating WEB, DB, and ADMIN traffic. |
| 05 | Allowed Traffic Validation | Required outbound connectivity, WAN pings, and DNS resolution. |
| 06 | Blocked Lateral Movement Validation | WEB client traffic to DB and ADMIN gateways was blocked and logged. |
| 07 | Admin Access Hardening | pfSense management restricted to ADMIN and blocked from WEB. |
| 08 | Logging and Monitoring Evidence | Firewall log entries and monitoring dashboard visibility. |
| 09 | Final Risk Reduction Summary | Summary of security controls and risk reduction achieved by the lab. |

## Tools And Technologies

- pfSense
- VirtualBox
- Kali Linux clients
- Segmented virtual networks
- Firewall aliases and rules
- DHCP scopes
- Firewall logs and monitoring dashboards

## Skills Demonstrated

- Network segmentation design
- Firewall policy implementation
- Least-privilege admin access design
- Lateral movement reduction
- Connectivity validation
- Log review and monitoring evidence
- Evidence portfolio organization

## Boundary

This is a controlled local lab, not a live production engagement or scan of a real company network. Production validation would require written authorization, approved scope, staging infrastructure, monitoring, and stop conditions.
