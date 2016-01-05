# OpenZonePlayer

## Idea

There are several Sonos-compatible software-based controllers, but apparently there is no software-based ZonePlayer compatible player so far. Can we cange that? (Or is https://github.com/henkelis/sonospy one? "Music served from Sonos can now be rendered locally via BRisa renderer" that is nice, but we want Sonos-compatible controllers play music on the OpenZonePlayer.)

According to [Wikipedia](https://en.wikipedia.org/wiki/List_of_UPnP_AV_media_servers_and_clients), "all Sonos Player Compononents (PLAY:3, PLAY:5, Connect, Connect:AMP, PLAYBAR)" are "UPnP media render hardware". So if the players are UPnP media renderers, why isn't there a ZonePlayer-compatible UPnP media renderer?

This is what I think would need to be done:
 1. Send SSDP broadcast messages to make the device discoverable by controllers
 2. Respond to UPnP messages in a ZonePlayer-like way, possibly using/building on https://github.com/hzeller/gmrender-resurrect or https://github.com/JiapengLi/OpenWrt-gmediarender (precompiled at https://forum.openwrt.org/viewtopic.php?pid=236110#p236110)
 3. Find a way to synchronize multiple players for multiroom experience

### Sonos-compatible software-based controllers

 * https://github.com/SoCo/SoCo Sonos Controller is a simple Python class that allows you to programmatically control Sonos speakers 
 * https://github.com/SoCo/socos Commandline tool for controlling Sonos devices
 
### To be investigated

  * https://github.com/henkelis/sonospy UPnP control point and Windows Media proxy for the Sonos multi-room audio system

This project is in no way affiliated with SONOS, Inc. and is using only publicly available information.
