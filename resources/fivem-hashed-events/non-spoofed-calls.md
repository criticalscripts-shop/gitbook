# Non-Spoofed Calls

You can listen to the following server event for when a non-spoofed call is detected.

A non-spoofed call is a hashed event triggered using its original (pre-hash) name.

```lua
AddEventHandler('cs-hashed-events:OnNonSpoofedCall', function(source, name, resource)
    -- (source) has triggered (name) event within (resource), do what you want with them.
end)
```
