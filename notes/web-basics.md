# Web Basics

## What Happens When You Type a URL

1. **DNS Lookup**
   - The browser asks DNS: “What IP address belongs to this domain?”
   - Example: google.com → 142.250.x.x

2. **TCP Connection**
   - Browser opens a connection to the server (3-way handshake).

3. **TLS Handshake (HTTPS)**
   - Encryption is negotiated.
   - Certificates are checked.

4. **HTTP Request**
   - Browser sends a request like:
     GET /index.html HTTP/1.1

5. **Server Processing**
   - Server processes the request (web server + backend).

6. **HTTP Response**
   - Server sends HTML, CSS, JS back.

7. **Browser Rendering**
   - Browser builds the page and displays it.

---

## Where Security Can Fail

### DNS
- DNS spoofing
- Malicious DNS servers

### Transport Layer
- Man-in-the-middle attacks
- Weak TLS configurations

### Web Server
- Misconfigured permissions
- Directory listing enabled

### Application Layer
- SQL Injection
- XSS
- Authentication bypass

### Client Side
- Malicious JavaScript
- Insecure cookies

---

## Why This Matters in Cybersecurity
Understanding this flow helps identify **where attacks occur** and **how to defend them**.4. **HTTP Request**
   - Browser sends a request like:
     GET /index.html HTTP/1.1

5. **Server Processing**
   - Server processes the request (web server + backend).

6. **HTTP Response**
   - Server sends HTML, CSS, JS back.

7. **Browser Rendering**
   - Browser builds the page and displays it.

---

## Where Security Can Fail

### DNS
- DNS spoofing
- Malicious DNS servers

### Transport Layer
- Man-in-the-middle attacks
- Weak TLS configurations

### Web Server
- Misconfigured permissions
- Directory listing enabled

### Application Layer
- SQL Injection
- XSS
- Authentication bypass


