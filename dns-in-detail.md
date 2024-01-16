# DNS in Detail
* Doman Name System

## TLD
* Top Level Domain

### gTLD
* Generic (.com, .org ...)

### ccTLD
* Country Code (.ca)

## Second Level Domain
* 63 characters

## Subdomain
* Can only be 253 characters

## Recond Types
* A Record: resolve to IPv4
* AAAA Record: IPv6
* CNAME: Conincal name, a pointer to another domain name
* MX: Mail Exchange records, servers that handle the mail (Good for phising)
* TXT: Text records, any text based can be used

## Making a DNS request

### 1. Check Cache 
### 2. Recursive DNS Server by ISP
### 3. Root DNS Server
### 4. Authoritative DNS Server, main server for the domain
### 5. Send back to recursive DNS server for ISP (DNS records have TTL), caching saves lives
