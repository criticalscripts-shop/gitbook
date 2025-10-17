---
description: Learn how to install the resource.
---

# Installation Instructions

{% stepper %}
{% step %}
### Download the resource

* Make sure you have [yarn](https://github.com/citizenfx/cfx-server-data/tree/master/resources/\[system]/\[builders]/yarn) in your `resources` folder.
* Download `cs-video-call` and place it in your `resources` folder.
{% endstep %}

{% step %}
### Ensure the resource

Add `ensure cs-video-call` to your server's configuration file before ensuring your phone.
{% endstep %}

{% step %}
### Hook your phone's resource

Edit your phone's `fxmanifest.lua` file and add the following at the end of of the file:

{% code title="fxmanifest.lua" %}
```
client_script '@cs-video-call/client/hooks/core.lua'
server_script '@cs-video-call/server/hooks/core.lua'
```
{% endcode %}
{% endstep %}

{% step %}
### Hook your phone's NUI

Edit your phone's NUI file (usually `index.html`) and add the following right before the `</body>` tag:

<pre><code><strong>&#x3C;script type="text/javascript" src="nui://cs-video-call/client/hooks/core.js">&#x3C;/script>
</strong></code></pre>
{% endstep %}

{% step %}
### Configure

Check the `config.lua` file inside `cs-video-call` for further configuration. Read through all options and their comments and adjust them to your setup and preferences.
{% endstep %}

{% step %}
### Setup your server's firewall

Open the required port (by default `34540`; incoming / inbound) in your firewall, on `UDP` protocol.

{% hint style="info" %}
If you are having issues getting a port open, you can use an [External Proxy Server](external-proxy-server.md).
{% endhint %}
{% endstep %}

{% step %}
### Start the resource

Run the following commands on the server console:

{% code title="FiveM Server Console" %}
```
refresh
ensure cs-video-call
```
{% endcode %}
{% endstep %}

{% step %}
### Fix your phone's animation loop

{% hint style="warning" %}
This is optional and you don't need to do anything unless you are experiencing an animation glitch.
{% endhint %}

If your phone uses an animation loop you may need to edit it (usually found in an `animation.lua` file) and add a `not CS_VIDEO_CALL.ACTIVE` check before playing an animation to ensure an animation glitch does not occur when the video call camera is opened.

### Restart your phone

Ensure your phone's resource via your server's console.
{% endstep %}
{% endstepper %}
