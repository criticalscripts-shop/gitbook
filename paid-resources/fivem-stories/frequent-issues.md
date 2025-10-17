---
description: Learn how to deal with frequent issues.
---

# Frequent Issues

<details>

<summary>I can use the stories app but when I try to view or upload a story, an error happens, why?</summary>

If your phone is of `fx_version cerulean`_,_ then you will have to route the stories' hosting server via **HTTPS**. You can do this by using a domain and Cloudflare.  Alternatively, you can change the `fx_version` of your phone to `bodacious`_._ If this was not your issue then the problem usually lies in **TCP** **blocking**, complex network setup or anti-DDoS protection. **Try a different port, preferably in a high range** to see if that will resolve your issue and **make sure that port is open for TCP protocol**.\
If that doesn't work then your best solution here may be to [externally host the stories' hosting server](external-hosting-server.md) in a different machine (for example a cheap VPS with enough bandwidth / network / storage to work within your own limits) that can handle the requirements.

</details>

<details>

<summary>I've done everything but I cannot see a stories app button, what's wrong?</summary>

Not seeing a stories app button is possibly related to the hook you are using. First make sure you are using the correct hook for the phone you have. Then make sure your phone events and DOM elements are properly reflected in the hook and that the hook is configured properly. Also note that some hooks add the stories application in the phone's application store rather than immediately adding it as an application.

</details>

<details>

<summary>My <strong>yarn</strong> is repeatedly trying to install the resource, what do I do?</summary>

This seems to be a current bug in the **yarn** resource related to `package.json` and the server's time zone related to the time zone of the system you copied the resource from.\
Edit `package.json` and just add or remove a space character, save it and the issue will go away.

</details>
