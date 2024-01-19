# Subdomain Enumeration
* Finding valid subdomanins for a domain
* Can be done via brute force, Open Source Intelligence (OSINT), and Virtual Host

## OSINT - SSL/TLS Certs
* Secure Sockets Layer/Transport Layer Security cert is create for domain by Certificate Authority (CA), the CA takes part in Certificate Transparency(CT) logs
* These logs are public to make sure no malicious or accidentally made certs are being used
* Can use `https://crt.sh/` to search domains for subdomains based on certs

## OSINT - Search Engines
* Can use search teams like `-site:domian site:*.domain` to find other sub domains and just these

## DNS Bruteforce
* Trying tens, hundreds, thousands, millions of different subdomains
* Can use a command for this, `dnsrecon`

## OSINT - Sublist3r
* Automated way of discovering subdomains

## Virtual Hosts
* some subdomains could be hosted on private DNS servers
* We can use the host header and change it to see if we can discover any other subdomains
* Can use `ffuf` to dod this 
