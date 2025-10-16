# Installation Instructions

{% stepper %}
{% step %}
### Download & place resource

Download `cs-hashed-events` and place it in your `resources` folder.
{% endstep %}

{% step %}
### Ensure resource

Add `ensure cs-hashed-events` to your server's configuration file before any other ensure.
{% endstep %}

{% step %}
### Include in fxmanifest.lua

Edit the `fxmanifest.lua` file of every resource in your server that executes Lua scripts and add:

```lua
shared_script '@cs-hashed-events/include.lua'
```
{% endstep %}

{% step %}
### Configure

Adjust the resource configuration via its `config.lua` file and ConVars.
{% endstep %}

{% step %}
### Restart

Restart your server.
{% endstep %}
{% endstepper %}

***
