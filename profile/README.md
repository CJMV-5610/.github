# Security Analysis of Client-Server Communication in Video Games
__Colin Greybosh, Jessica Zhang, Mahmoud Sobier, Vishnu Penubarthi__

## Minetest NMPR Fork
A Dockerized version of the Minetest Network Multiplayer Release (NMPR).

The `docker-compose.yml` file included in this repo contains configuration settings
that pertain to launching an instance of the Minetest NMPR to act as a server, an
instance of the `udp_proxy` image built from the UDP Proxy repo, and a second instance
of the Minetest NMPR to act as a client.

## UDP Proxy
A Python application that acts as a man-in-the-middle for any communication done with
the Minetest server, whether that communication come from a local source (within the
Docker network) or externally (within the host machine or client with remote access).
