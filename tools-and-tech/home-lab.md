---
title: Home Lab Gear and Software
layout: page
parent: Tools and Tech
nav_order: 2
---

# Home Lab Gear and Software

## Compute/Storage Hardware
I use a custom built server runing Unraid. I've been using Unraid since 2009 and it has consistently gotten better year over year. It comes with a Docker engine built in, the ability to use KVM for virtual machines, and a huge community behind it. I highly recommend it. I'll eventually add more detail here on the hardware and how I use this. 

Currently this server is running:
- Intel Core i5-8400 (6 Cores @ 2.8GHz)
- 32GB DDR4
- Gigabyte Z370P Motherboard
- LSI 9201-16i(SAS2116) PCIe disk controller
    - Firmware is running in IT mode or JBOD mode. No RAID.
- 2 x Intel DC S3610 400GB SSD (6Gb/s SATA)
- 10 x Seagate IronWolf NAS 10TB HDD (256MB Cache, 7200 RPM, 6Gb/s SATA)
- Rosewill 4U server case with 12 x hot swap 3.5" drive bays
    - Essentially [this case](https://www.neegg.com/rosewill-rsv-l4412u-black/p/N82E16811147330), but I've had this for 10+ years, so I cannot confirm if this is still the same.

The two Intel datacenter SSDs are part of the cache pool, which is where all of my containers and virtual machines run. 

The ten Seagate drives are all part of the array, which is where all my other data is stored. Of those ten drives, two are considered partity devices and eight are data devices. This gives me a total of 80TB of usable space in the array.

## Network Hardware
- Fortigate 60E
- Fortiswitch 124F - main rack switch
- Fortiswitch 108F - desk rack switch
- Ruckus R650 - running Unleashed firmware

The two Fortiswitches are a recent addition. I didn't have any previous experience with them and wanted to learn, so I swapped the two Cisco switches for these. Working well so far. The integration with the Fortigate is very nice. Running 1Gb fiber interconnects between the Fortiswitches with copper uplinks to the Fortigate.

## Monitoring and Graphing
This is one of the things I really enjoy playing with. Telegraf and InfluxDB are great and everyone knows Grafana. Very useful opensource projects. More to come on these tools. 

- [Telegraf](https://hub.docker.com/_/telegraf)
- [InfluxDB](https://hub.docker.com/_/influxdb)
- [Grafana](https://hub.docker.com/r/grafana/grafana)
- [Uptime Kuma](https://github.com/louislam/uptime-kuma)
- [Mosquitto (MQTT broker)](https://hub.docker.com/_/eclipse-mosquitto)

## Automation
I don't have a ton of things to automate, but sometimes you just want a project to learn how things work. I've been using a lot of Ansible and Jenkins to automate Docker container deployments, Linux configuration, and updates, but nothing groundbreaking. I need to write a small article on how I use this.

## File Syncronization
[Syncthing](https://docs.syncthing.net/) - This really deserves a separate write up under the projects section.

## Media Server
[Emby](https://emby.media/) - I was a loyal Plex user for a very long time, but several years ago I made the decision to move away from Plex to something that only ran locally on my home network and didn't require a login to any outside service to function. I can use Emby with no internet connection at all, which is not something you can do with Plex (at least this was the case when I switched). 

## Home Automation
~~[Homebridge](https://github.com/homebridge/docker-homebridge) - lets me bring non-HomeKit enabled devices into HomeKit. All of my other devices, lamps, cameras, etc. are HomeKit enabled. I have since stopped using this, but I've been playing around with HomeAssistant recently. Nothing permanent, just an experiment right now.~~

I'm just now starting to think about moving my existing home automation tools over to [Home Assistant](https://www.home-assistant.io/). I have it deployed and have a few things in there, but haven't cut everything over just yet. Still getting my feet wet, but I like the idea that I can host this locally and restrict access to it. 

## Remote Access
I used a pretty simple [Wireguard](https://www.wireguard.com/) setup for a long time, but have recently switched to [Tailscale](https://tailscale.com). Still testing right now, but it has been great so far. Extremely simple to setup and has some great features. 

## Ad Blocking/DNS
[Pihole](https://hub.docker.com/r/pihole/pihole) - I run two instances of this, each on separate hardware. Both are running on docker. 

## Logging
[Dozzle](https://dozzle.dev/) - great for reviewing docker container logs. Connects to docker.sock to automatically discover running containers and display logs for those containers in a nice web interface.

## Virtualization
I made the decision a while ago to switch everything I could over to docker containers. However, I've recently found myself in need of some testing VMs, so I've added a small ProxMox machine to my homelab (Intel NUC, nothing huge). Nothing permanent running on this, but it's been handy to have this around. My Home Assistant VM is deployed on the Unraid server since that has more horsepower and is intended to be permanent.

## Cloud Hosting
[Linode](https://www.linode.com/) - I have used DigitalOcean, Vultr, and Amazon Lightsail, but my favorite so far has been Linode. They were recently acquired by Akamai, but no negative changes have been made as far as I am aware. 

I have also recently been using [Hetzner](https://www.hetzner.com/). Time will tell which one comes out as my favorite. 
