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


General Administration Commands (Useful for Network/Firewall Admins):

    Check Network Interfaces:

    bash

ip a

Display Routing Table:

bash

ip route

Add a New Route:

bash

sudo ip route add 192.168.2.0/24 via 192.168.1.1

Check Active Connections:

bash

sudo netstat -tuln

Check Port Usage:

bash

sudo ss -tuln

Traceroute to an IP or domain:

bash

traceroute google.com

Ping to check connectivity:

bash

ping 8.8.8.8

Check FirewallD rules (if you are using FirewallD):

bash

sudo firewall-cmd --list-all

Add a permanent rule to FirewallD:

bash

sudo firewall-cmd --permanent --add-port=22/tcp
sudo firewall-cmd --reload

Systemd Network Configuration (show status of networking):

bash

sudo systemctl status systemd-networkd

Check NAT table (for both iptables-nft and nftables):

bash

    sudo iptables -t nat -L
    sudo nft list table ip nat

Handy Tools for Network Administration:

    tcpdump (network packet analysis):

    bash

sudo tcpdump -i eth0

nmap (network scanning tool):

bash

nmap -sP 192.168.1.0/24

ipcalc (subnet calculator):

bash

ipcalc 192.168.1.1/24

dig (DNS lookup):

bash

dig google.com

curl (make HTTP requests):

bash

curl -I http://example.com
