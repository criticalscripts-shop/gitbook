# Important Information

* The player will be asked for microphone approval, if they deny, their voice will not be recorded in stories. If they mistakenly deny, they will need to reset it (for now this is done by deleting the file `%AppData%\CitizenFX\media_access.json`).
* When recording a story, the voice is recorded by the player's system default microphone. This cannot be changed.
* Only the voice of the player recording is recorded. This cannot be changed.
* The recording determinates whether the player is talking using the built-in native. If you are using an external VoIP such as TokoVoip or similar you will need to edit the hook to correctly determine when the player is talking.
* A player recording a story cannot move. This is default GTA:V camera behavior. You can try using experimental camera mode which allows the player to move, however it might not be as smooth as the native one.
* Video render lag / freezes may be caused in very high resolutions or in very low-spec systems.
* The story recording works using game capture (similar to screenshot-basic), whatever it's on the game is recorded. That includes visual settings / mods, game drawings / UIs but not NUIs.
* If your server is running behind a reverse proxy that you have no control over and cannot handle an extra TCP port as required by the resource, your only option may be to externally host the stories' hosting server in a different machine (for example a cheap VPS with enough bandwidth / network / storage to work within your own limits).
* When a story is being uploaded or viewed by a player, like any other video-upload service, the player's upload / download speed is being used and network / bandwidth is consumed on the hosting server as well.
* If your hosting server host does not offer unlimited bandwidth or has a low network limit you are advised to periodically check your usage statistics if you have a lot of players uploading and viewing stories. Also make sure to check your storage if you have a ton of stories being uploaded and are not being cleaned up.
* The resource is using FiveM's KV storage to store the metadata of the saved stories, if you are using a shared multi-server setup this may cause an issue and you may want to set `sv_kvsName` console variable to something unique for your server.
* There are checks in place to ensure that the recorded video and the in-game location are legitimate and are coming from the game itself, however since the client sends them, they cannot be fully trusted.
* The stories are deleted (as per configuration) when the resource starts, so stories storage cleanup depends on how often you restart your server or the resource.
