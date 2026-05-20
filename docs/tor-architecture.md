# Tor Architecture

# Introduction

Tor (The Onion Router) is a decentralized anonymity network designed to protect user privacy and online identity.

Tor routes internet traffic through multiple volunteer-operated servers called relays.

This process helps hide:

- User IP addresses
- Browsing activity
- Geographic location

---

# Main Goals of Tor

## Privacy

Tor helps users browse anonymously.

## Anonymity

Network traffic becomes difficult to trace.

## Anti-Censorship

Users can bypass internet restrictions in some regions.

---

# Core Components

# 1. Entry Guard Node

The first relay in the Tor circuit.

Responsibilities:
- Receives user traffic
- Knows user's IP address
- Does NOT know final destination

---

# 2. Middle Relay Node

Intermediate relay between entry and exit nodes.

Responsibilities:
- Pass encrypted traffic
- Hide traffic origin
- Increase anonymity

---

# 3. Exit Node

Final relay before traffic reaches destination.

Responsibilities:
- Sends traffic to internet
- Can see unencrypted traffic
- Does NOT know original user identity

---

# Circuit Construction

Tor creates random circuits using multiple relays.

Typical path:

User → Entry Node → Middle Node → Exit Node → Website

Each node only knows limited information.

---

# Layered Encryption

Tor uses layered encryption similar to onion layers.

Each relay removes one encryption layer.

This prevents single nodes from knowing:
- complete route
- source
- destination

---

# Advantages

- Strong privacy
- Anonymous browsing
- Distributed infrastructure
- Open-source technology

---

# Limitations

- Slower internet speed
- Some websites block Tor traffic
- Exit nodes may inspect unencrypted traffic

---

# Conclusion

Tor remains one of the most important privacy technologies used for anonymous communication and research.
