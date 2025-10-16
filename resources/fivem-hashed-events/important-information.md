# Important Information

* By default the resource whitelists internal events, game events, txAdmin and vMenu events.
* For any non-Lua resource (e.g. C# / JS) that trigger events, network or not, outside of its own resource, the events will need to be whitelisted.
* To put it simply, if a "non-hashed" resource needs to communicate with a "hashed" resource via events, network or not, the events will need to be whitelisted.
* If everything is set up as intended and you have not missed anything, you can be confident non-spoofed calls are deliberate.
* This resource is purely an extra friction layer for event discovery and abuse.
  * It does not prevent exploitation by a determined adversary.
  * It does not guarantee secrecy of event names under targeted analysis.
  * It does not replace proper server-side validation, permissions, or rate limiting.
* Use this as one layer in a defense-in-depth strategy, not a remedy for all modder problems.

