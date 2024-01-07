# Hell's tunnel

Hell's tunnel is a layer 7 protocol that evades detection from traffic analysis and firewalls. It works by wrapping TCP/UDP data in a E2EE tunnel to the server over HTTPS WebSocket protocol.

This protocol can protect and hide transmitted data from being discovered by censors, traffic analysis and/or blue teams. Only the client and server knows about the true nature of the connection. Not only connections to remote addresses can be routed by the protocol, but also connections to another client can be routed as long as both clients are on the same server.

The name "Hell's tunnel" comes from it's purpose, which is to make sure the data survives and remain undetected while going though "hell". It also comes from it's alternate purpose, which is to serve as a backdoor/pivot into a client or the internal network, opening up a tunnel from "hell". 

## Project structure

The file [SPECIFICATION.txt](SPECIFICATION.txt) contains the final specifications of the tunneling protocol.

The directory [specification-breakdown](specification-breakdown/) contains a layman breakdown of the specification and it's various features.

## Features

- [ ] Outbound tunnel to a server
- [ ] Reverse tunneling (Useful for pivoting through networks)
- [ ] Hidden listener through IP whitelist/blacklist

## Possible usages

- Pivoting through a network by hiding traffic as HTTPS or browsing a CDN protected site (Any cdn that support WebSockets will do)

- Securely tunnel into a network, like a home network setup.

- Securely tunnel out of a network, like a heavily censored country and evade detection from the network specific censors like GFW.

- Protect a reverse shell connection or a foothold into a network.

- Stealthily exfiltrate data from a target during a red team exercise.
