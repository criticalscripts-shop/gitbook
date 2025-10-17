---
description: Learn how to configure the resource via console variables.
---

# ConVars

You can set the following ConVars in your server's configuration file using `setr` (e.g. `setr s_hashed_events_enabled true`).



* `cs_hashed_events_enabled`
  * An easy way to control whether the resource will be enabled or not, after it has been included to every resource.



* `cs_hashed_events_server_whitelist`
  * A comma-separated list of server events that should be allowed to pass without hashing, for non-Lua resources.



* `cs_hashed_events_client_whitelist`
  * A comma-separated list of client events that should be allowed to pass without hashing, for non-Lua resources.



* `cs_hashed_events_emojify`
  * Whether you want the event hashing to be emoji-based, this will cause the events to show up as question marks in the network event log.
