---
description: Learn important information about the resource.
---

# Important Information

* The resource is optimized with range synchronization and assets are loaded only when the player is around an active vehicle.
* Very low-spec computers may experience a more downgraded experience.
* If you want to ensure the resource, you are advised to stop the playback in all active vehicles first to avoid crashes.
* Colliding replacers will prioritize the ones that are closer to the player and may also replace objects nearby if they happen to have the same texture, this is not something that can be changed and you can avoid it by not having the same vehicles in the same area and use vehicle-specific texture replacements instead of generic objects.
* The resource works by using a vehicle's plate as an identifier. When two or more vehicles have the same plates, only one of them will work. This is true even for vehicles that are on different buckets.
* In the default configured entries, adjusting the content time for buffering and syncing is turned off as it is not mandatory for a great experience. This feature is complicated and may not always work as intended, therefore it is advised to enable it only in time-critical content.
* Some triangle / black textures may appear in monitors when there are a lot of players around, that seems to be a game texture bug.
* Minor crackling may be audible on certain songs when the camera is moved due to limitations imposed upon spatial audio.
* If content fails to load or play for any reason for the player who is controlling the UI, it will stop for everyone. If content fails to load or play for any reason for a player who is only viewing / listening, it may attempt to reload for them.
* There are checks in place in an attempt to verify that the transmitted data (titles, thumbnail URL, icon, etc.) are legitimate and are coming from the within resource itself, however since the client sends it, they cannot be fully trusted.
