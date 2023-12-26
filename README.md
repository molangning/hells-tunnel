# Hell's tunnel

Hell's tunnel is a layer 7 protocol that evades detection from traffic analysis and firewalls. It works by wrapping TCP/UDP data in a E2EE encrypted tunnel to the server over HTTPS WebSocket protocol.

The file [SPECIFICATION.txt](SPECIFICATION.txt) contains a rough sketch of the tunneling protocol while the directory [SPECIFICATIONS](SPECIFICATIONS/) contains the final specifications to the protocol

## Features

- [ ] Outbound tunnel to a server
- [ ] Reverse tunneling (Useful for pivoting through networks)

## Possible usages

- Pivoting through a network by hiding traffic as HTTPS or browsing a CDN protected site (Any cdn that support WebSockets will do)

- Securely tunnel into a network, like a home network setup.

- Securely tunnel out of a network, like a heavily censored country and evade detection from the network specific censors like GFW.

- Protect a reverse shell connection or a foothold into a network.

- Stealthily exfiltrate data from a target during a red team exercise.