---
title: Home Lab Gear and Software
layout: page
parent: Tools and Tech
nav_order: 2
---

# Home Lab Gear and Software

## Compute/Storage Hardware
I use a custom built server runing Unraid. I've been using Unraid since 2009 and it has consistently gotten better year over year. It comes with a Docker engine built in, the ability to use KVM for virtual machines, and a huge community behind it. I highly recommend it. I'll eventually add more detail here on the hardware and how I use this. 

## Network Hardware
- Cisco 2960X-24PSQ-L - Main rack switch
- Cisco 2960CG-8TC-L - Desk rack switch
- PC Engines APU2 running pfSense
- Ruckus R650 - running Unleashed firmware

## Monitoring and Graphing
This is one of the things I really enjoy playing with. Telegraf and InfluxDB are great and everyone knows Grafana. Very useful opensource projects. More to come on these tools. 

- [Telegraf](https://hub.docker.com/_/telegraf)
- [InfluxDB](https://hub.docker.com/_/influxdb)
- [Grafana](https://hub.docker.com/r/grafana/grafana)
- [Uptime Kuma](https://github.com/louislam/uptime-kuma)
- [Mosquitto (MQTT broker)](https://hub.docker.com/_/eclipse-mosquitto)
- [cloudflare-speedtest-mqtt](https://github.com/ccmpbll/cloudflare-speedtest-mqtt)

## File Syncronization
[Syncthing](https://docs.syncthing.net/) - This will be getting its own write up under the projects section.

## Media Server
[Emby](https://emby.media/) - I was a loyal Plex user for a very long time, but several years ago I made the decision to move away from Plex to something that only ran locally on my home network and didn't require a login to any outside service to function. I can use Emby with no internet connection at all, which is not something you can do with Plex (at least this was the case when I switched). 

## Home Automation
[Homebridge](https://github.com/homebridge/docker-homebridge) - lets me bring non-HomeKit enabled devices into HomeKit. All of my other devices, lamps, cameras, etc. are HomeKit enabled. 

## Remote access
[Wireguard](https://www.wireguard.com/) - this also needs its own write up. 

## Ad blocking/DNS
[Pihole](https://hub.docker.com/r/pihole/pihole) - I run two instances of this, each on separate hardware. Both are running on docker.

## Logging
[Dozzle](https://dozzle.dev/) - great for reviewing docker container logs. Connects to docker.sock to automatically discover running containers and display logs for those containers in a very nice web interface.

## Virtualization
As hard as it might be to believe, there are no virtual machines running in my homelab. I made the decision a while ago to switch everything I could over to docker containers. However, I do find myself needing to test something in a VM from time to time. When that happens, I usually just spin up a VM on my Unraid box.

## Cloud Hosting
[Linode](https://www.linode.com/) - I have used DigitalOcean, Vultr, and Amazon Lightsail, but my favorite so far has been Linode. They were recently acquired by Akamai, but no negative changes have been made as far as I am aware. 
