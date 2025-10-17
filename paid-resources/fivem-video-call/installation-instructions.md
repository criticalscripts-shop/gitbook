---
description: Learn how to install the resource.
---

# Installation Instructions

{% stepper %}
{% step %}
### Download the resource

* Make sure you have [yarn](https://github.com/citizenfx/cfx-server-data/tree/master/resources/\[system]/\[builders]/yarn) in your `resources` folder.
* Download `cs-stories` and place it in your `resources` folder.
{% endstep %}

{% step %}
### Ensure the resource

Add the following line to your server's configuration file before ensuring your phone:

ensure cs-video-call
{% endstep %}

{% step %}
### Add hooks to phone resource files

Edit your phone's _**\_\_resource.lua**_ or _**fxmanifest.lua**_ file and add the following:

* As the last client script: '@cs-video-call/client/hooks/core.lua'
* As the last server script: '@cs-video-call/server/hooks/core.lua'
{% endstep %}

{% step %}
### Add NUI script to phone

Edit your phone's NUI file (usually _**index.html**_) and add this before :
{% endstep %}

{% step %}
### Configure cs-video-call

Check the _**config.lua**_ file inside _**cs-video-call**_ for further configuration and read through all options and their comments as some are very important for the setup process. Adjust them to your setup and preferences.
{% endstep %}

{% step %}
### Open required UDP port (internal solution)

Given you're using the internal solution, open the **required port** (by default **34540**; **incoming** - **inbound**) in your firewall on **UDP** protocol.
{% endstep %}

{% step %}
### Refresh and ensure

Run the command refresh and the command ensure cs-video-call and wait until **yarn** finishes the installation.
{% endstep %}

{% step %}
### Prevent animation glitch (if needed)

If your phone uses an animation loop you may need to edit it (usually found in an **animation.lua** file) and add a not CS\_VIDEO\_CALL.ACTIVE check before playing an animation to ensure an animation glitch does not occur when the video call camera is opened.
{% endstep %}

{% step %}
### Final step

Ensure your phone.
{% endstep %}
{% endstepper %}
