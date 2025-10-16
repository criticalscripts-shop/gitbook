# Installation Instructions

{% stepper %}
{% step %}
### Download and place resource

Download _**cs-ves**_ and place it in your _**resources**_ folder.
{% endstep %}

{% step %}
Add the following to your server configuration:

{% code title="server.cfg" %}
```
ensure cs-ves
```
{% endcode %}
{% endstep %}

{% step %}
Add Ace permission for admin access to the /ves command (this can be changed via integration files):

```
add_ace group.admin cs-ves.control allow
```
{% endstep %}

{% step %}
Check and adjust the _**config.lua**_ file inside _**cs-ves**_ to enable the vehicle models you want to be available.
{% endstep %}

{% step %}
Run:

```
refresh
ensure cs-ves
```
{% endstep %}
{% endstepper %}
