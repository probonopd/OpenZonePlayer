# OpenZonePlayer

## Idea

There are several Sonos-compatible software-based controllers, but apparently there is no software-based ZonePlayer compatible player so far. Can we cange that? (Or is https://github.com/henkelis/sonospy one? "Music served from Sonos can now be rendered locally via BRisa renderer")

According to [Wikipedia](https://en.wikipedia.org/wiki/List_of_UPnP_AV_media_servers_and_clients), "all Sonos Player Compononents (PLAY:3, PLAY:5, Connect, Connect:AMP, PLAYBAR)" are "UPnP media render hardware". 

This is what would need to be done:
 1. Send SSDP broadcast messages to make the device discoverable by controllers
 2. Respond to UPnP messages in a ZonePlayer-like way

### Sonos-compatible software-based controllers

 * https://github.com/SoCo/SoCo Sonos Controller is a simple Python class that allows you to programmatically control Sonos speakers 
 * https://github.com/SoCo/socos Commandline tool for controlling Sonos devices
 
### To be investigated

  * https://github.com/henkelis/sonospy UPnP control point and Windows Media proxy for the Sonos multi-room audio system

This project is in no way affiliated with SONOS, Inc. and is using only publicly available information.
