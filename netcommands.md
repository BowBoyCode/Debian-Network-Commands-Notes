Here is the rewritten list formatted in **Markdown** for your GitHub:

```markdown
### Networking Commands:

- `ip addr` – Show IP addresses and network interfaces
- `ip link` – Display or configure network interfaces
- `ip route` – Show or manipulate the routing table
- `ping <host>` – Test connectivity to a host
- `traceroute <host>` – Trace the route packets take to a host
- `nslookup <domain>` / `dig <domain>` – Query DNS records for a domain
- `netstat` / `ss` – Display network connections, routing tables, and interface statistics
- `ifconfig` – Display or configure network interfaces (older tool, often replaced by `ip`)
- `iwconfig` – Configure wireless interfaces
- `hostname` – Show or set the system's hostname
- `nmap <host>` – Network exploration and security auditing
- `curl <URL>` – Transfer data to/from a server
- `wget <URL>` – Download files from the web
- `tcpdump` – Capture network packets
- `nmcli` – NetworkManager command-line tool for managing network connections

---

### General Administration Commands (Useful for Network/Firewall Admins):

- `ip a` – Check Network Interfaces
- `ip route` – Display the Routing Table
- `sudo ip route add 192.168.2.0/24 via 192.168.1.1` – Add a New Route
- `sudo netstat -tuln` – Check Active Connections
- `sudo ss -tuln` – Check Port Usage
- `traceroute google.com` – Traceroute to an IP or Domain
- `ping 8.8.8.8` – Ping to Check Connectivity
- `sudo firewall-cmd --list-all` – Check FirewallD Rules (if you are using FirewallD)
- `sudo firewall-cmd --permanent --add-port=22/tcp && sudo firewall-cmd --reload` – Add a Permanent Rule to FirewallD
- `sudo systemctl status systemd-networkd` – Show Status of Systemd Network Configuration
- `sudo iptables -t nat -L` / `sudo nft list table ip nat` – Check NAT Table for iptables-nft and nftables

---

### Handy Tools for Network Administration:

- `sudo tcpdump -i eth0` – Capture Network Packets
- `nmap -sP 192.168.1.0/24` – Network Scanning Tool
- `ipcalc 192.168.1.1/24` – Subnet Calculator
- `dig google.com` – DNS Lookup
- `curl -I http://example.com` – Make HTTP Requests
```

This Markdown format will work well on GitHub or any other markdown-supported platform, providing clear sections and command details.
