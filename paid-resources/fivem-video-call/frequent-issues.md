---
description: Learn how to deal with frequent issues.
---

# Frequent Issues

<details>

<summary>I can perform a video call but when the other player opens their camera all I see is a black screen, why?</summary>

Black screen issue is usually related to **UDP blocking**, complex network setup or anti-DDoS protection. **Try a different port, preferably in a high range** to see if that will resolve your issue and **make sure that port is open for UDP protocol**.\
If that doesn't work then your best solution here may be to [externally host the video call's proxy server](external-proxy-server.md) in a different machine (for example a cheap VPS with enough bandwidth / network to work within your own limits) that can handle the requirements.

</details>

<details>

<summary>I've done everything but I cannot see a video call button, what's wrong?</summary>

Not seeing a video call button is possibly related to the hook you are using.\
First make sure you are using the correct hook for the phone you have.\
Then make sure your phone events and DOM elements are properly reflected in the hook and that the hook is configured properly.

</details>

<details>

<summary>My <strong>yarn</strong> is repeatedly trying to install the resource, what do I do?</summary>

This seems to be a current bug in the **yarn** resource related to `package.json` and the server's time zone related to the time zone of the system you copied the resource from.\
Edit `package.json` and just add or remove a space character, save it and the issue will go away.

</details>
