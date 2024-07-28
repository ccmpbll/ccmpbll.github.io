---
title: Prusa Enclosure Setup and Upgrades
layout: post
parent: Projects
nav_order: 1
---

# Prusa Enclosure Setup and Upgrades

![](/assets/images/prusa_enclosure.jpg)

## Summary
After upgrading from my beloved Prusa MK3S+ to a MK4, I decided the enclosure I built from Ikea Lack tables was no longer going to work. It was inexpensive and it was a fun build, but I needed more room inside the enclosure. Enter the official Prusa Enclosure. See below for some of my efforts to set the enclosure up to my liking.

## General Setup

### Details

I failed to take any pictures during the assembly process, but as with all things Prusa, the documentation is well done and I had no issues. The only part that I chose not to use was the printed feet for the enclosure. My enclosure sits on top of my small server rack, so I want to eliminate as much vibration and noise as possible. I chose to go with 2 packs of Sorbothane feet and stuck them directly to the bottom of the enclosure. They're working very well so far. I would recommend using the 70 Duro version as they are a bit more rigid and less likely to get completely squished by the weight of the enclosure. I put one on each corner and another 4 in the bottom center of the enclosure, directly under where the printer and quartz slab sit.

The acrylic used for the sides and doors has a ton of static after you remove the protective paper and it attracts dust like crazy. I found this MG Chemicals cleaner that will remove the static and clean the surface. Worked extremely well.

I won't bother creating a separate section for this, but its definitely worth mentioning. The hinged lid add on for the Prusa Enclosure is well worth the little effort and filament it requires. You can find details [HERE](https://www.printables.com/model/273426-hinged-lid-for-adding-mmu2s-to-original-prusa-encl). It doesnt require any additional parts, only what is included with the enclosure kit.

![](/assets/images/enclosure_hinged_lid.jpg)

### Parts
- [1.5"x.5" 70 Duro Sorbothane feet](https://www.amazon.com/dp/B019O68IY0)
- [MG Chemicals Antistatic Plastic Cleaner](https://www.amazon.com/dp/B072QWBJ9K)

## LED Lighting for Enclosure

### Details

I added LEDs to my old enclosure and found it extremely useful, so I knew I had to have lighting for this enclosure as well. I was able to reuse a lot of the parts from the old setup, but added a few upgrades along the way.

The first problem was figuring out how to mount the aluminum channels to the inside of the enclosure. Since I chose to use the hinged lid modification, I wanted something that didn't attach to the lid itself. After a bit of investigation, I found a [model on Printables](https://www.printables.com/model/333871-original-prusa-enclosure-unofficial-version) that I could import into Fusion and model on top of. That gave me the correct dimensions for everything. I created this model that uses existing holes in the enclosure and holds the aluminum channel up against the inside of the enclosure. 

![](/assets/images/enclosure_lights_model_1.jpg)![](/assets/images/enclosure_lights_model_2.jpg)
![](/assets/images/enclosure_lights_model_3.jpg)

The next step was installing the LEDs in the channels and wiring everything up. I failed to take pictures of this part, but the LEDs were cut to size and stuck to the inside of the channels. I used two pieces of wire about 4in long for each end of the LED strips, crimped on the JST connectors, and soldered them onto the LED strips. The JST connectors allows me to replace one section of LEDs at a time without having to disassemble or desolder things.

Now it was time to tackle cabling and powering everything. I really didn't want to have these LEDs powered by the printers power supply this time. I did that with the old enclosure, but the printer had to be on for the lights to be on and that's not very useful if I want to remove the printer and work on the inside of the enclosure. I dug around on Amazon for a while and found a 24v power supply intended to be used with LEDs. This was very easy to wire up. Just needed a pair of low voltage power pigtails and another couple of JST connectors.

The last thing was to integrate this with OctoPrint so I could control the LEDs separately from the printer. I already used the Tasmota plugin and an EZplug+ from TH3D to control the power to the printer and this is what I used to control the LEDs as well. I added another EZPlug+ to the Tasmota plugin and can power on the lights and printer independently from one another. 

Here you can see the final product. They're extremely bright and are working very well so far. Very happy with how this turned out.

![](/assets/images/enclosure_lights_1.jpg)![](/assets/images/enclosure_lights_2.jpg)

### Parts
- [16" Aluminum Channel with Diffuser for LED Strips](https://www.amazon.com/dp/B0C6GKXNWQ)
- [16.4' Insanely bright LED Strip](https://www.amazon.com/dp/B0BYNS9YYQ)
- [2 pin JST Connectors](https://www.amazon.com/dp/B07QKBKNC1)
- [18 AWG Silicone Stranded Wire](https://www.amazon.com/dp/B01708AYYQ)
- [4' Male/Female Power Cable Pigtails](https://www.amazon.com/dp/B0CWV1MP2J)
- [Armacost 36W 24V LED Power Supply](https://www.amazon.com/dp/B08YS6GMP6)
- [TH3D EZPlug+ Wifi Tasmota Smart Plug](https://www.th3dstudio.com/product/ezplug-open-source-wifi-smart-plug/)




## Spool Holders and Filament Passthrough

### Details
Coming Soon!

### Parts
- [PC4-M10 Fittings](https://www.amazon.com/dp/B095P7Z62Y)
- [PTFE Tubing](https://www.amazon.com/dp/B01CUPV9KC)
- [15x6x2mm magnets for spool holders](https://www.amazon.com/dp/B0B7X3RJ54)

## Logitech C920 Mount

### Details

The last piece I needed to create was a mount for a C920 Logitech camera I use for OctoPrint. The Prusa Enclosure has plenty of holes and places to mount things, so it was just a matter of designing something that would fit with my existing camera. I drew this up in Fusion in just a few minutes and printed it out in black PETG. Added some M3 screws and nuts and it was done. No complaints so far.

![](/assets/images/c920_mount_model.jpg)![](/assets/images/c920_mount.jpg)