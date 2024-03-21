4# Linux

## cron
* MIN (minute) HOUR (hour) DOM (day of month) MON (month) DOW (day of week) CMD

## Commands I Learned
* `file`: determine the type of a file
* `fg`: bring process to fore ground
* `history`: gets a history of commands ran
* `kill <pid> found via ps aux`: kill a process 
* `nmap <ip>`: short for network map, can run to see what services are running (install via homebrew)
* `man` gives a manual on how to use a command
* `python3 -m http.server` simple http server where you run and serve files from current directory
* `ps`: process command
* `top`: get all the top running processes using memory and such
* `wget` to fetch things from sites

## Operators
* `&`: run programs in background of terminal
* `&&`: combine multiple commands together
* `>`: redirector
* `>>`: redirector but also appends

## Commone Directories
* `/etc`: common for system files by operating system
* `/var`: variable data, contains application logs
* `root`: home for root use
* `tmp`: short for temporary, volatile (good for pen testing as any user can write to this)

## Passive Reconnaissance
* `whois <url>`
* `nslookup` Name server look up
  * `nslookup -type=<A ip4, AAAA ip6, MX mail server> <url> <public dns>`
* `dig <DNS> <type>` Domain Information Groper

## Active Recon
* `ping <ip address>`
  * `ping -c <num times to ping> <ip address>` can ping for a set amount of times
* `traceroute <ip/url>` will give you all the routers inbetween an ip/url, using increasing numbers of ttl packets, starting at 1
* `telnet <ip> <port>` we can send messages to get more information about the server
  * once connected we can send in a `GET / HTTP/1.1` to extract information
* `nc` or netcat, supports TCP and UDP protocols, can be a client or a server.
  * `nc <ip> <port>`
* `nmap`
  * `nmap <ip1> <ip2>` to scan multiple
  * `nmap <ip.low-high>` to scan range
  * `nmap <ip>/<subnet>` to scan subnet
  * `nmap -iL <text list>` list of targets
  * `nmap -sL -n <ip range>` will list the actual ips it will scan
  * `nmap -sn TARGETS` to discover online hosts without port scanning
  * `nmap -PR` indicates only ARP scans
  * `nmap -PE` indicates only ICMP echo scans
  * `nmap -PP` indicated only ICMP timestamp scans
  * `nmap -PM` indicated only address mask scans
