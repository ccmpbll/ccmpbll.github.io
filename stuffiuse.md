---
title: Stuff I Use
layout: page
nav_order: 3
---

# List of software/tools/stuff I use

## 3D Printing and Design
- Printer - [Prusa MK3S+](https://www.prusa3d.com/category/original-prusa-i3-mk3s/)
- Slicer Software - PrusaSlicer and [SuperSlicer](https://github.com/supermerill/SuperSlicer)
- 3D Design/CAD - [Fusion360](https://www.autodesk.com/products/fusion-360/personal)
- Digital Calipers - [Neiko 01407A 6in Stainless Steel Digital Calipers](https://www.amazon.com/Neiko-01407A-Electronic-Digital-Stainless/dp/B000GSLKIW/) - Yes you can buy better calipers, but not for the money. My advice: spend the extra money and get the 12in version. 
- Filament - We could talk about this all day. My favorites are Polymaker, PrintedSolid, and Prusament. I just realized they all start with P. Weird.
- Also, [OctoPrint](https://octoprint.org/) is a must.

## Home lab
This is a big list, so I'm going to break it up into smaller groups. 

### Compute/Storage Hardware
Details coming soon.

### Network Hardware
- Cisco 2960X-24PSQ-L - Main rack switch
- Cisco 2960CG-8TC-L - Desk rack switch
- PC Engines APU2 running pfSense
- Ruckus R650 - running Unleashed firmware

### Monitoring and Graphing
- [Telegraf](https://hub.docker.com/_/telegraf)
- [InfluxDB](https://hub.docker.com/_/influxdb)
- [Grafana](https://hub.docker.com/r/grafana/grafana)
- [Uptime Kuma](https://github.com/louislam/uptime-kuma)
- [Mosquitto (MQTT broker)](https://hub.docker.com/_/eclipse-mosquitto)
- [cloudflare-speedtest-mqtt](https://github.com/ccmpbll/cloudflare-speedtest-mqtt)

### File Syncronization
- [Syncthing](https://docs.syncthing.net/) - this deserves its own write up. 

### Media Server
- [Emby](https://emby.media/) - I was a loyal Plex user for a very long time, but several years ago I made the decision to move away from Plex to something that only ran on my home network and didn't require any login to any outside service to operate. I can use Emby with no internet connection at all, which is not something you can do with Plex. 

### Home Automation
- [Homebridge](https://github.com/homebridge/docker-homebridge) - lets me bring non-HomeKit enabled devices into HomeKit. 

### Remote access
- [Wireguard](https://www.wireguard.com/) - this also needs its own write up. 

### Ad blocking/DNS
- [Pihole](https://hub.docker.com/r/pihole/pihole) - I run two instances of this, each on separate hardware. Both are running on docker.

### Logging
- [Dozzle](https://dozzle.dev/) - great for reviewing docker container logs.

### Virtualization
- As hard as it might be to believe, there are no virtual machines running in my homelab. I made the decision a while ago to switch everything I could over to docker containers. 

### Cloud Hosting
- [Linode](https://www.linode.com/) - I have used DigitalOcean, Vultr, and Amazon Lightsail, but my favorite so far has been Linode. They were recently acquired by Akamai, but no negative changes have been made as far as I am aware. 
