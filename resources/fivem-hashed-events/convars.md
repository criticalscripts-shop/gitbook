# ConVars

You can set the following ConVars in your server's configuration file using setr (e.g. setr cs\_hashed\_events\_enabled true).

* cs\_hashed\_events\_enabled
  * \[ true | false ] An easy way to control whether the resource will be enabled or not, after it has been included to every resource.
* cs\_hashed\_events\_server\_whitelist
  * \[serverEvent1,serverEvent2] A comma-separated list of server events that should be allowed to pass without hashing, for non-Lua resources.
* cs\_hashed\_events\_client\_whitelist
  * \[clientEvent1,clientEvent2] A comma-separated list of client events that should be allowed to pass without hashing, for non-Lua resources.
* cs\_hashed\_events\_emojify
  * \[ true | false ] Whether you want the event hashing to be emoji-based, this will cause the events to show up as ?????? in the network event log.
