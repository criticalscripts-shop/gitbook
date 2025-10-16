# Installation Instructions

{% stepper %}
{% step %}
### Preparation

* Make sure you have [yarn](https://github.com/citizenfx/cfx-server-data/tree/master/resources/\[system]/\[builders]/yarn) in your `resources` folder.
* Download `cs-stories` and place it in your `resources` folder.
{% endstep %}

{% step %}
### Enable the resource

* Add `ensure cs-stories` to your server's configuration file before ensuring your phone.
{% endstep %}

{% step %}
### Hook the phone resource

* Edit your phone's `__resource.lua` or `fxmanifest.lua` file and add `@cs-stories/client/hooks/core.lua` as the last client script and `@cs-stories/server/hooks/core.lua` as the last server script.
{% endstep %}

{% step %}
### Add the NUI script

* Edit your phone's NUI file (usually `index.html`) and add: right before `</body>`.
{% endstep %}

{% step %}
### Configure

* Check the `config.lua` file inside `cs-stories` for further configuration. Read through all options and their comments and adjust them to your setup and preferences.
{% endstep %}

{% step %}
### Firewall / Port

* Given you're using the internal solution, open the required port (by default `35540`; incoming/inbound) in your firewall on TCP protocol.
{% endstep %}

{% step %}
### Start the resource

* Run the command `refresh` and then `ensure cs-stories`.
{% endstep %}

{% step %}
### Animation loop fix (if needed)

* If your phone uses an animation loop you may need to edit it (usually found in an `animation.lua` file) and add a `not CS_STORIES.ACTIVE` check before playing an animation to ensure an animation glitch does not occur when the video call camera is opened.
{% endstep %}

{% step %}
### Final check

* Ensure your phone.
{% endstep %}
{% endstepper %}
