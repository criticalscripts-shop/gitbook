# Expansions

`cs-hall` does **NOT** support any streaming services by default, out-of-the-box you can only queue URLs with embeddable video elements (e.g. self-hosted). In addition to that you may use controllers' expansions to expand on the supported media sources at your own risk and discretion, you can find more in our [extra-hac GitHub](https://github.com/criticalscripts-shop/extra-hac/tree/main/cs-hall/controllers) and in our [Discord](https://criticalscripts.shop/discord) community.&#x20;

To install an expansion controller, follow these steps:

{% stepper %}
{% step %}
### Copy all the contents of the controller

Copy all the contents of the controller you wish to install, not the file itself, but its contents.
{% endstep %}

{% step %}
### Open expansions file

Navigate to `cs-hall/client/dui/javascript/controllers/` and open the `expansions.js` file.
{% endstep %}

{% step %}
### Paste the contents of the controller

Paste the contents of the controller in your `expansions.js` file and save it.
{% endstep %}

{% step %}
### Restart the resource

Type `ensure cs-hall` in your server's console.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Please be mindful of the content you stream since your players also stream it through their clients.&#x20;
{% endhint %}
