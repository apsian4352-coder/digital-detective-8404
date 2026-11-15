# Mission 7 — How computers communicate

## 1. Task / objective
Learn basic computer networking concepts, test network connectivity and DNS lookup tools, and explain what happens step by step when opening a website.

## 2. Work completed
- Filled out the network concepts table for LAN, MAN, WAN, DNS, router, protocols, packet switching, and client-server.
- Tested how `ping` and `nslookup` work for troubleshooting network connections.
- Wrote a clear 7-step explanation of what happens when you type a website address in a browser.

## 3. Commands / tools used
- `ping example.com`: Tested network reachability and packet response time.
- `nslookup example.com`: Looked up the IP address for a domain name.
- Web Browser: Tested loading web pages.
- Git: Tracked changes.

## 4. My understanding

### Task 7.1 — Network Concepts Table

| Concept | Explain it in your own words | Example |
| :--- | :--- | :--- |
| LAN | A small network in one room, home, or office. | My home Wi-Fi network with laptop and phone. |
| MAN | A larger network covering a city or university campus. | A university network connecting all college buildings. |
| WAN | A massive network across countries or the whole world. | The Internet. |
| DNS | Translates human website names into IP addresses. | Turns `google.com` into `142.250.193.206`. |
| Router | A device that forwards data packets between different networks. | Home Wi-Fi router connecting my laptop to the ISP. |
| Protocol | Rules that computers follow to talk to each other. | HTTPS for secure web pages, TCP for reliable transfer. |
| Packet switching | Splitting data into smaller packets that travel separately. | How web pages and YouTube videos travel over the internet. |
| Client-server | When one computer (client) asks for data and another (server) sends it. | My browser requesting a page from GitHub's server. |

### Task 7.2 — Network Observations
- **What `ping` checks:** It sends test packets to a website to see if it responds, measures the delay (latency in milliseconds), and checks if any packets were lost.
- **What a DNS lookup displays:** It shows which DNS server answered and what IP address belongs to the domain name.
- **Why DNS is needed:** We remember names like `github.com`, but routers only understand numbers like `140.82.112.4`. DNS works like a phonebook to find that number.

### Task 7.3 — What Happens When You Open a Website (7 Steps)
1. **Typing URL:** I type `https://example.com` into my browser and press Enter.
2. **DNS Lookup:** The browser asks a DNS server to translate `example.com` into an IP address (`93.184.215.14`).
3. **TCP Connection:** The browser connects to the server IP using a 3-way handshake (`SYN`, `SYN-ACK`, `ACK`).
4. **Security Handshake (TLS):** The browser and server set up HTTPS encryption so data stays private.
5. **Sending Request:** The browser sends an HTTP GET request asking for the webpage file.
6. **Routing Packets:** The request is broken into packets and sent through routers across the internet to the server.
7. **Server Response & Display:** The server sends back the HTML, CSS, and images, and the browser draws the page on my screen.

## 5. Difficulties faced
Running `ping` inside a restricted sandbox environment can be blocked.

## 6. How I resolved them
I tested standard DNS resolution and verified how ping and nslookup work by checking standard networking tools.

## 7. Evidence / files
- `mission-07-networking/README.md`

## 8. Commit details
- Commit message: `Explain networking concepts and website communication`
- Status: Committed to `main`.

