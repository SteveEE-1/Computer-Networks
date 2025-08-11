# Networking

## Protocols


### DNS

**Domain name System**, When a domain name example `google.com` it goes to the DNS server and fetches the appropriate ip address of that particular domain. 
**Recursive resolution** = DNS server does all the work of resolving the name.

The **+** in your tcpdump shows the **"Recursion Desired"** flag is set — so you're asking the `DNS server to resolve everything and return just the IP`.

### UDP

**User Datagram Protocol** ,It directly does transmission of data without any connection to that server or system. Connectionless protocol.

### TCP

**Transmission control protocol**, `Transport Layer`.Connects with the particular system or server and check if they system acknowledges the particular request. It follows a `Three way handshake`


### HTTPS

**Hyper Text Transfer Protocol** , Its a more secure way connection via web servers and client. It encrypts the data using `TLS/SSL` encryption methods. So a attacker cant view the data during the transmission.
`Application Layer`. This is a security protocol.


### Simple Network Management Protocol (SNMP)

Is a network protocol used for monitoring and managing devices on a network. SNMP can reset a password on a network device or change its baseline configuration. Can be used for reporting how much bandwidth is being used 


### Internet Control Message Protocol (ICMP)  

Its used for checking data transmission errors across the the network.
Used to troubleshoot the network and latency by pinging. 


### Secure File Transfer Protocol (SFTP)

Mainly used in file transfer uses SSH protocol for file transfer. It encrypts using **AES(Advanced encryption standard)** so it cant be intercepted and read.



### DHCP (Dynamic Host Configuration Protocol)

It assigns a devices its IP address and other configuration on a network.

### ARP (Address Resolution Protocol)

It translates the IP address in the data packets into **MAC** addresses so that the devices can be found in the local network. Does not have port number since its layer 2 protocol.


### Telnet

Used to remotely connect with devices over network. Sends information via clear text.

### SSH (Secure Shell)

Securily connect to a remote system. Serves authentication and encryptions.

### IMAP (Internet Message Access Protocol)

IMAP is used for incoming email. Donwloads headers of emails and message content. Once the mail is downloaded it doesnt get deleted from the server and can be accessed again from multiple devices.

# PORTS

| **Protocol/Service**      | **Port Number** | **Transport** | **Encryption**            |
| ------------------------- | --------------- | ------------- | ------------------------- |
| **DHCP (Server)**         | 67              | UDP           | ❌                         |
| **DHCP (Client)**         | 68              | UDP           | ❌                         |
| **Telnet**                | 23              | TCP           | ❌                         |
| **SSH**                   | 22              | TCP           | ✅ (Encrypted)             |
| **SFTP**                  | 22              | TCP           | ✅ (via SSH)               |
| **POP3**                  | 110             | TCP/UDP       | ❌                         |
| **POP3S (POP3 over SSL)** | 995             | TCP/UDP       | ✅ (SSL/TLS)               |
| **IMAP**                  | 143             | TCP           | ❌                         |
| **IMAPS (IMAP over SSL)** | 993             | TCP           | ✅ (SSL/TLS)               |
| **SMTP**                  | 25              | TCP/UDP       | ❌                         |
| **SMTPS (SMTP with TLS)** | 587             | TCP/UDP       | ✅ (TLS)                   |
| **HTTP**                  | 80              | TCP           | ❌                         |
| **HTTPS**                 | 443             | TCP           | ✅ (SSL/TLS)               |
| **DNS**                   | 53              | TCP/UDP       | ❌ (typically unencrypted) |

