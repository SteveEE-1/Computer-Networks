
# 📡 Networking Devices

## 📘 Basic Key Notes

- **Hosts**: Any devices that send or receive network traffic (e.g., clients, servers).
- **IP Address**: A unique identifier assigned to each host in a network.
- **Network**: Enables the transmission of data packets between hosts.

---

## 🔁 Repeater
- A repeater regenerates and amplifies signals to extend the physical reach of a network.
- Commonly used in large or long-distance networks to maintain signal strength.

---

## 🔗 Hub
- Also called a **multiport repeater**.
- Connects multiple devices in a network.
- **Limitation**: Broadcasts incoming data to **all connected devices**, regardless of the destination.
- Operates at **Layer 1 (Physical Layer)** of the OSI model.

---

## 🧱 Bridge
- Connects two network segments, usually two hubs.
- Has **exactly two ports**.
- Learns the MAC addresses of connected devices to intelligently forward traffic.
- If both sender and receiver are on the same side, the bridge doesn't forward data to the other side.
- Operates at **Layer 2 (Data Link Layer)**.

---

## 🔀 Switch
- Connects multiple devices within the **same network** (like a smart hub).
- Sends data **only to the intended recipient device**, not to all devices.
- Combines the features of a hub and a bridge.
- Maintains a MAC address table to optimize data flow.
- Operates at **Layer 2**, but some modern switches support **Layer 3 routing**.

**Example**:  
All systems below are part of the same network (192.168.10.x):  
- System A: `192.168.10.1`  
- System B: `192.168.10.2`  
- System C: `192.168.10.3`  

---

## 🌐 Router
- Connects **different networks** and directs data between them.
- Provides routing, traffic management, filtering, redirection, and basic firewall security.
- Maintains a **routing table** to decide the best path for packet delivery.
- Assigned an IP address on each network it connects — this is called the **gateway** address.
- Operates at **Layer 3 (Network Layer)** of the OSI model.



