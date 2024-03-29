Uno
========

This is the server module for CS 3230 Group 1

### Running the module

NodeJS must first be installed on the system. Navigate to the "server" directory (this
can be found on the `base_server` branch of this repository) and run `node server.js`.
Then, from an IDE or `.jar` file, start this server module listening on the same machine
(`Uno.jar`). Alternately, you can upload the `.jar` file to the server and run it
using _**TODO**_

### Writing server code

* _**TODO**_

### The following message types are handled by the server:

* _LOGIN_

```json
{
  "type": "login",
  "message": 
    {
      "username": "<user display name (must be unique)",
      "password": "<admin password>"  // this entry is optional
    }
}
```
* _CHAT_

```json
{
  "type": "chat",
  "message": "<chat text>"
}
```

* _WHOIS_

```json
{
  "type": "whois"
}
```

* _APP_

```json
{
  "type": "application",
  "message": 
    {
      "module": "Uno",
      <other data as defined by the API>
    }
}
```

### The following message types may be sent from the server:

* _APP_
* _WHOIS_
* _ACK_
* _ERROR_
