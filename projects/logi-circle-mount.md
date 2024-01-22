---
title: Custom Mount For Logitech Circle View Camera
layout: post
parent: Projects
nav_order: 1
---

# Custom Mount For Logitech Circle View Camera

## Summary
I like hummingbirds. I think they're fascinating. Unfortunately, I have to work and I don't have time to stare out the window all day waiting on them to come to the feeder.

That's where the camera comes in, but there are limited options if you want cameras that integrate with HomeKit (more on that later). I settled on the Logitech Circle View camera. Decent reviews, a company I know, and it works with HomeKit. Perfect...Except the mount is ~~garbage~~ not ideal for my needs. After some deliberation, I decided to remove the stand that came on the camera and just make my own. 

This little project also has the added benefit of having a camera pointed toward my front yard and driveway, so I end up catching people coming and going along with the hummingbirds.

## Parts/Design
I chose this suction cup base from RAM Mounts and it is excellent. Best suction cup base mount I've used. You can get one here: [Amazon Link](https://www.amazon.com/RAM-Twist-Lock-RAP-224-1U-Compatible-Components/dp/B001447JYG)

I took the hole spacing measurements from the base and took a ton of measurements of the camera itself with my digital calipers and came up with this design in Fusion360. The base comes with two screws to attach your accessory, so I measured those and recessed them into the mount so they're flush with the top. I sliced it up in PrusaSlicer and printed it in [Polymaker Carbon Fiber PLA](https://us.polymaker.com/products/polylite-pla-cf). Print time was about 1h 24m. 

![](/assets/images/logimount.gif)

The only other parts needed were an M2x16 socket head cap screw and an M2 nut to attach the camera to the mount. 

## Update - January 2024
As mentioned above, I chose to print this part in carbon fiber PLA. This turned out to be a bad choice. The sun coming through the window in the afternoon turned out to be much hotter than I assumed. The heat caused the part to deform so that the camera was pointing down at the ground. I reprinted the part, this time in carbon fiber PETG. Hopefully this will perform much better.

## Finished Product
![](/assets/images/cameramount.jpeg)

{% include youtube.html id="4HzgGr8CyRk" %}
