# LAN Network Scanner (Python)

A multithreaded LAN network scanner built in Python to detect live hosts on a given subnet and scan common open TCP ports.

This project uses ICMP ping for host discovery and TCP socket connections for port scanning.

---

## Features

- Scans a given subnet (CIDR format)
- Detects live hosts using ping
- Scans common ports (22, 80, 443, 8000)
- Uses multithreading for faster scanning
- Displays results in a clean table format

---

## Technologies Used

- Python 3
- ipaddress
- subprocess
- socket
- threading

---

## How It Works

1. Generates all IP addresses in the given subnet.
2. Pings each IP to check if the host is alive.
3. If alive, scans common TCP ports using socket connection.
4. Prints results in a table.

---

## Usage

Run the scanner using:

```bash
python lan_network_scanner.py <subnet>
```

Example:

```bash
python lan_network_scanner.py 192.168.1.0/24

```
