---
description: Learn how to install the resource.
---

# Installation Instructions

{% stepper %}
{% step %}
### Download the resource

Download `cs-ves` from your keymaster and place it in your `resources` folder.
{% endstep %}

{% step %}
### Ensure the resource

Add the following to your server configuration:

{% code title="server.cfg" %}
```
ensure cs-ves
```
{% endcode %}
{% endstep %}

{% step %}
### Setup Ace permission

Add this to your server configuration so Ace admins can access the `/ves` command:

{% code title="server.cfg" %}
```txt
add_ace group.admin cs-ves.control allow
```
{% endcode %}

{% hint style="info" %}
This check can be changed by modifying **`cs-hall/lntegration/server.lua`**.
{% endhint %}
{% endstep %}

{% step %}
### Configure vehicles

Open `config.lua` inside `cs-ves` and enable the entries for the vehicle models you want the VES to be available.&#x20;

{% hint style="info" %}
You can find more vehicle models in our [extra-hac GitHub](https://github.com/criticalscripts-shop/extra-hac/tree/main/cs-ves/entries) and in our [Discord](https://criticalscripts.shop/discord) community.
{% endhint %}
{% endstep %}

{% step %}
### Start the resource

Run the following commands on the server console:

{% code title="FiveM Server Console" %}
```
refresh
ensure cs-ves
```
{% endcode %}
{% endstep %}
{% endstepper %}
