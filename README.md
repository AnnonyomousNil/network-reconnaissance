# network-reconnaissance
**TASK 1**

**Nmap** is a free and open-source tool used for **network reconnaissance**. It helps in **scanning** or performing **service detection** in a network to find **vulnerabilities**.

---

## How to Use Nmap

### 1. Find Your IP Address Range

First, we will find our IP address range.

Open a terminal on Linux and type:

```bash
ifconfig
```

Now, from the results, note the IP range. For example:

192.168.230.0 - 192.168.230.255

### 2. Perform a TCP SYN Scan
Use the following command to find open ports in the range:

```bash
nmap -sS 192.168.230.0/24
```

### Example Scan Results
As seen in the output, the following ports are open:

- 902/tcp – Commonly used for VMware virtual machines

- 912/tcp – Often used by Acronis or proprietary applications

- 5357/tcp – Used for Web Services Discovery (WSD)

- 53/tcp – Used for Domain Name System (DNS) on 192.168.230.2

### Security Risks of Open Ports
- Open ports are potential attack vectors.

- Many exploits target specific services running on default ports.

- Open ports can pose a security risk because they can act as entry points for unauthorized access to a system or network.

- If ports are not properly configured and protected, hackers can exploit vulnerabilities and potentially gain control of the system.
