# Important Information

* The video call will not work without the proxy server, direct P2P is not given as an option in order to protect players' anonymity.
* Besides your proxy server's network speeds which must match the amount of maximum active transmissions you want to have (you can limit those in the configuration), you will also need to consider bandwidth consumption if that is not unlimited by your host.
* Video render lag / freezes may be caused in very high resolutions or in very low-spec systems.
* When video call is active, the player who transmits the video cannot move. This is default GTA:V camera behavior. You can try using experimental camera mode which allows the player to move, however it might not be as smooth as the native one.
* The video call works using game capture (similar to _screenshot-basic_), the player sees whatever it's on the game of the other player. That includes visual settings / mods, game drawings / UIs but not NUIs.
* If your server is running behind a reverse proxy that you have no control over and cannot handle an extra UDP port as required by the resource, your only option may be to externally host the video call's proxy server in a different machine (for example a cheap VPS with enough bandwidth / network to work within your own limits) that can handle the requirements.
* When a player initiates a video call, it will consume approximately 2mbps of their upload speed for the transmission and when they are in a call and the other player initiates a video call it will consume approximately 2mbps of their download speed.
* Your players may be prompted by their Windows Firewall to allow a connection the first time a video call happens, this is due to the WebRTC protocol connection and cannot be circumvented.
* There are checks in place to ensure that the transmitted video feed is legitimate and is coming from the game itself, however since the client sends it, it cannot be fully trusted.
