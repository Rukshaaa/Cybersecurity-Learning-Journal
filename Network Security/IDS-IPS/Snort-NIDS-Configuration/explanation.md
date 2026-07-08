# Snort Configuration Explanation

## HOME_NET

HOME_NET was defined as 10.10.0.0/16 because this represents the internal company network. These systems are owned by the organization and should be monitored for suspicious activity.

## EXTERNAL_NET

EXTERNAL_NET was configured as anything outside HOME_NET because external traffic comes from untrusted networks such as the internet.

## DMZ Servers

The DMZ subnet 172.16.10.0/24 contains public-facing servers. These systems are separated from internal resources because they are exposed to external users.

## HTTP_SERVERS

The web server was grouped separately because HTTP/HTTPS traffic requires different monitoring rules compared to other systems.

## Port Groups

Ports 80 and 443 were assigned to HTTP services because they represent web traffic.
