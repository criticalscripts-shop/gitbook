# Installation Instructions

{% stepper %}
{% step %}
### Download the resource

Download `cs-hall` from your keymaster and place it in your `resources` folder.
{% endstep %}

{% step %}
### [Install `cs-stream`](#user-content-fn-1)[^1]

Download `cs-stream` from: [https://github.com/criticalscripts-shop/cs-stream](https://github.com/criticalscripts-shop/cs-stream)

Place it in your `resources` folder and add the following to your server configuration file:

```txt
ensure cs-stream
```

{% hint style="warning" %}
If you choose not to use it you will have to change the default configuration as the default spotlight object is an addon and the default screen for some locations is from The Cayo Perico Heist DLC which your server may not be on.
{% endhint %}
{% endstep %}

{% step %}
### Ensure the resource

Add the following to your server configuration file:

```txt
ensure cs-hall
```
{% endstep %}

{% step %}
### Setup Ace permission

Add this to your server configuration so Ace admins can access the `/hall` command:

```txt
add_ace group.admin cs-hall.control allow
```

{% hint style="info" %}
This check can be changed by modifying **`cs-hall/lntegration/server.lua`**.
{% endhint %}
{% endstep %}

{% step %}
### Configure locations

Open `config.lua` inside `cs-hall` and enable the entries for the locations you want the hall to be available.&#x20;

{% hint style="info" %}
You can find more locations in our [extra-hac GitHub](https://github.com/criticalscripts-shop/extra-hac/tree/main/cs-hall/controllers) and in our [Discord](https://criticalscripts.shop/discord) community.
{% endhint %}
{% endstep %}

{% step %}
### Start the resource

Run the following commands on the server console:

```txt
refresh
ensure cs-hall
```
{% endstep %}
{% endstepper %}



[^1]: This step is optional but recommended.
