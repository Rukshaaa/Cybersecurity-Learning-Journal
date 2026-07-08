# Snort NIDS Configuration Project

## Overview

This project demonstrates the design and configuration of a Snort Network Intrusion Detection System (NIDS) for a simulated enterprise network.

The goal of this project was to design a network architecture, identify critical assets, define monitored networks, and configure Snort rules to detect suspicious traffic patterns.

## Network Architecture

The simulated organization contains:

- Internal user network
- Mobile BYOD network
- DMZ server environment
- Secure database network
- Cloud-based external API communication

The network is protected by an edge firewall, with Snort positioned as a network monitoring component to analyze incoming and outgoing traffic.

## Network Segments

| Network | Subnet | Purpose |
|---|---|---|
| Internal Users | 10.0.10.0/24 | Employee workstations |
| Mobile BYOD | 10.0.20.0/24 | Personal mobile devices |
| DMZ / Servers | 172.16.50.0/24 | Public-facing services |
| Database Network | 172.16.60.0/24 | Protected database systems |

## Servers Monitored

### Web Server
- Host: Nginx Web Server
- IP: 172.16.50.10
- Services:
  - HTTP (80)
  - HTTPS (443)

### DNS Server
- Host: BIND9 DNS
- IP: 172.16.50.53
- Service:
  - DNS (53)

### Mail Server
- Host: Postfix Mail
- IP: 172.16.50.25
- Services:
  - SMTP (25)
  - Submission (587)

### Database Server
- Host: PostgreSQL Database
- IP: 172.16.60.100
- Service:
  - PostgreSQL (5432)

## Security Objectives

Snort was configured to:

- Monitor suspicious network activity
- Detect unauthorized access attempts
- Identify abnormal traffic patterns
- Alert on potential reconnaissance activity
- Protect critical server infrastructure


## Skills Demonstrated

- Network segmentation
- IDS configuration
- TCP/IP networking
- Security monitoring
- Firewall concepts
- Snort rule development
