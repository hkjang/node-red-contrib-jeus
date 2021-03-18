node-red-contrib-jeus
================

Node-RED node for jeus


## Install

To install the stable version use the `Menu - Manage palette - Install`
option and search for node-red-contrib-jeus, or run the following
command in your Node-RED user directory, typically `~/.node-red`

    npm install node-red-contrib-jeus

## Wrapper nodejs jeus lib
- https://www.npmjs.com/package/jeus

## Example

```javascript
var msg = {};
msg.api = 'command'
msg.url = 'http://localhost:9736/jsonCommand/command.json';
msg.auth = {
    username : USERNAME,
    password : PASSWORD
}
msg.params = {
    "jeusadmin": {
        "command": "server-info",
        "options":[
            "-server server1",
            "-state"
        ],
        "argument": null
    }
};

return msg;
```
## Details
- https://technet.tmaxsoft.com/upload/download/online/jeus/pver-20170202-000001/reference-book/ch04.html#jeusadmin-json-support
