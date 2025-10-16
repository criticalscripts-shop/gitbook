# Installation Instructions

{% stepper %}
{% step %}
### Download and place resource

Download _**cs-hall**_ and place it in your **resources** folder.
{% endstep %}

{% step %}
### Optional: cs-stream

Download _**cs-stream**_ resource from: https://github.com/criticalscripts-shop/cs-stream

Place it in your **resources** folder and add the following to your server configuration file:

```txt
ensure cs-stream
```

This is optional but recommended. If you choose not to use it you will have to change the default configuration as the default spotlight object is an addon and the default screen for some locations is from The Cayo Perico Heist DLC which your server may not be on.
{% endstep %}

{% step %}
### Ensure cs-hall

Add the resource to your server configuration:

```txt
ensure cs-hall
```
{% endstep %}

{% step %}
### Ace permission for admins

Add this to your server configuration so Ace admins can access the /hall command:

```txt
add_ace group.admin cs-hall.control allow
```

This check can be changed by modifying **integration/server.lua**.
{% endstep %}

{% step %}
### Configure locations

Open **config.lua** inside **cs-hall** and enable the entries for the locations you want the hall to be available.
{% endstep %}

{% step %}
### Start resource

Run the following commands on the server console:

```txt
refresh
ensure cs-hall
```
{% endstep %}
{% endstepper %}
