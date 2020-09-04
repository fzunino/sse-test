# Server-Sent Events Example

Node.js example app to try out SSE.

Based on https://www.digitalocean.com/community/tutorials/nodejs-server-sent-events-build-realtime-app with some fixes applied.

Adds Message Id (`id:`) and Custom Event types (`event:`)

## Install & Run

* Run
```
$ npm install
$ node server.js
```

* Connect to `EventSream`
```
$ curl  -H Accept:text/event-stream http://localhost:4000/events
```

* Push Events
```
$ curl -X POST  -H "Content-Type: application/json"  -d '{"momma": "swamp_princess", "eggs": 40, "temperature": 32}' -s http://localhost:4000/nest
```



