# Networking Basics

## What Is Network Traffic?
Network traffic is the flow of data between a client (your computer) and a server over a network.

This data is broken into packets and sent across the network using protocols like TCP/IP.

---

## Simple Network Traffic Flow

Client (Browser)
        |
        v
   DNS Server
        |
        v
   Web Server
        |
        v
   Application
        |
        v
Client (Response)

---

## Step-by-Step Traffic Flow

1. **User enters a URL**
   - Example: https://example.com

2. **DNS Lookup**
   - The browser asks a DNS server for the IP address of the domain.

3. **TCP Connection**
   - A connection is established between client and server.

4. **TLS Handshake (HTTPS)**
   - Encryption is negotiated to secure the communication.

5. **HTTP Request**
   - The browser sends a request (GET/POST).

6. **Server Processing**
   - The web server and application process the request.

7. **HTTP Response**
   - Data (HTML, CSS, JS) is sent back to the client.

8. **Rendering**
   - The browser displays the page.

---

## Where Security Can Be Observed

- DNS traffic can be monitored or spoofed
- TLS encrypts data in transit
- Firewalls inspect incoming and outgoing packets
- IDS/IPS systems analyze traffic patterns
- Logs capture request and response activity

---

## Cybersecurity Relevance
Understanding traffic flow helps identify:
- Where attacks occur
- Where to monitor traffic
- How tools like Wireshark capture packets
