---
description: Learn important information about the resource.
---

# Important Information

* The resource is optimized with range synchronization and assets are loaded only when the player is around an active location.
* Very low-spec computers may experience a more downgraded experience.
* If you want to ensure the resource, you are advised to stop the playback in all active locations first to avoid crashes.
* The default configuration requires the _**cs-stream**_ resource which can be [downloaded here](https://github.com/criticalscripts-shop/cs-stream), started before `cs-hall` resource.
* In the most default configured entries, adjusting the content time for buffering and syncing is turned off as it is not mandatory for a great experience. This feature is complicated and may not always work as intended, therefore it is advised to enable it only in time-critical content (e.g., a cinema).
* Some triangle / black textures may appear in monitors when there are a lot of players around, that seems to be a game texture bug.
* Minor crackling may be audible on certain songs when the camera is moved due to limitations imposed upon spatial audio.
* If content fails to load or play for any reason for the player who is controlling the UI, it will stop for everyone. If content fails to load or play for any reason for a player who is only viewing / listening, it may attempt to reload for them.
* The resource is using FiveM's KV storage to store settings and queue for all locations, if you are using a shared multi-server setup this may cause an issue and you may want to set `sv_kvsName` console variable to something unique for your server.
* There are checks in place in an attempt to verify that the transmitted data (titles, thumbnail URL, icon, etc.) are legitimate and are coming from within the resource itself; however since the client sends it, they cannot be fully trusted.

