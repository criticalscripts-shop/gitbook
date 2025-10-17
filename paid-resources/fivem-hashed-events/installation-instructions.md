---
description: Learn how to install the resource.
---

# Installation Instructions

{% stepper %}
{% step %}
### Download the resource

Download `cs-hashed-events` and place it in your `resources` folder.
{% endstep %}

{% step %}
### Ensure the resource

Add `ensure cs-hashed-events` to your server's configuration file **before any other ensure**.
{% endstep %}

{% step %}
### Include in Lua resources

Edit the `fxmanifest.lua` file of every resource in your server that executes Lua scripts and add:

```lua
shared_script '@cs-hashed-events/include.lua'
```
{% endstep %}

{% step %}
### Adjust configuration

Adjust the resource configuration via its `config.lua` file and [ConVars](convars.md).
{% endstep %}

{% step %}
### Restart server

Restart your server.
{% endstep %}
{% endstepper %}
