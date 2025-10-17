---
description: Learn how to use an external proxy server.
---

# External Proxy Server

{% hint style="warning" %}
This is intended only for experienced developers.
{% endhint %}

If you choose not to use the integrated proxy server you can self-host an external proxy server.\
To do so, follow the instructions below.

{% stepper %}
{% step %}
### Download

Download the external proxy server through our [GitHub](https://github.com/criticalscripts-shop/cs-video-call-eps).
{% endstep %}

{% step %}
### Install

Run `npm install` in the EPS[^1] directory and wait until it completes.
{% endstep %}

{% step %}
### Configure

Read through all options and their comments inside its `config.js` file as they are very important for the setup process, adjust them to your setup and preferences.
{% endstep %}

{% step %}
### Run

Run `node server.js` in the EPS[^1] directory and **do not close the console window**.

{% hint style="info" %}
You can use [pm2](https://pm2.keymetrics.io/docs/usage/quick-start/) to make sure the EPS[^1] runs all the time.
{% endhint %}
{% endstep %}

{% step %}
### Configure your FiveM server

Add the EPS[^1] server's IP address in the `sv_proxyIPRanges` property in your server's configuration file.
{% endstep %}
{% endstepper %}



[^1]: External Proxy Server
