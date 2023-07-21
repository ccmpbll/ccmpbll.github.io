---
layout: page
title: Stuff I Use
---

## 3D Printing and Design
- Printer - Prusa MK3S+
- Slicer Software - PrusaSlicer and SuperSlicer
- 3D Design/CAD - Fusion360
- Digital Calipers - [Neiko 01407A 6in Stainless Steel Digital Calipers](https://www.amazon.com/Neiko-01407A-Electronic-Digital-Stainless/dp/B000GSLKIW/) - Yes you can buy better calipers, but not for the money. My advice: spend the extra money and get the 12in version. 
- Filament - We could talk about this all day. My favorites are Polymaker, PrintedSolid, and Prusament. I just realized they all start with P. Weird.
- Also, OctoPrint is a must.

## Home lab
This is a big list, so I'm going to break it up into smaller groups. 

### Compute/Storage Hardware
Details coming soon.

### Network Hardware
- Cisco 2960X-24PSQ-L - Main rack switch
- Cisco 2960CG-8TC-L - Desk rack switch
- PC Engines APU2 running pfSense
- Wireless hardware is currently a Netgear Orbi setup, but that's in the process of changing.

### Monitoring and Graphing
- Telegraf
- InfluxDB
- Grafana
- Uptime Kuma
- Mosquitto (MQTT broker)
- [cloudflare-speedtest-mqtt](https://github.com/ccmpbll/cloudflare-speedtest-mqtt)

### File Syncronization
- Syncthing - this deserves its own write up. 

### Media Server
- Emby - I was a loyal Plex user for a very long time, but several years ago I made the decision to move away from Plex to something that only ran on my home network and didn't require any login to any outside service to operate. I can use Emby with no internet connection at all, which is not something you can do with Plex. 

### Home Automation
- Homebridge - lets me bring non-HomeKit enabled devices into HomeKit. 

### Remote access
- Wireguard - this also needs its own write up. 

### Ad blocking/DNS
- Pihole - I run two instances of this, each on separate hardware. Both are running on docker.

### Logging
- Dozzle - great for reviewing docker container logs.

### Virtualization
- As hard as it might be to believe, there are no virtual machines running in my homelab. I made the decision a while ago to switch everything I could over to docker containers. 

### Cloud Hosting
- Linode - I have used DigitalOcean, Vultr, and Amazon Lightsail, but my favorite so far has been Linode. They were recently acquired by Akamai, but no negative changes have been made as far as I am aware. 
