
# MQTT PoC using Mosca.js

MQTT is a machine-to-machine (M2M)/"Internet of Things" connectivity protocol. 

It was designed as an extremely lightweight **publish/subscribe** messaging transport. 

It is useful for connections with remote locations where a small code footprint is required and/or network bandwidth is at a premium.

MQTT messaging protocol:

![diagram](./MQTT%20protocol.png)

## Prerequisites

- Install Mosca globally: `npm install mosca pino -g`
- Install Client dependencies: `npm install`


## Run unauthorized Mosca broker

Run `mosca -v | pino`


## Mosca Authorization & Authentication

`https://github.com/mcollina/mosca/wiki/Mosca-as-a-standalone-service.#authorization`

Run the broker with: `mosca -v --credentials ./credentials.json | pino`

Run the client with environment variables  for `username` and `password`.


## Run Client

Run the client with `node index.js`, setting environment variables if needed for Mosca authentication.


## Extra details..

`https://github.com/mqttjs/MQTT.js#connect`
