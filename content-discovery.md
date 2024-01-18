# Content Discovery
* In this case we are not talking about obvious things to find
* Manually, Automated, OSINT (Open Source Intelligence)

## Manual 
### robots.txt
* Restricts what can't be searched, which could be valuable places to explore

### Favicon
* We can curl the favicon link and then run via `md5sum` to get a hash and search in https://wiki.owasp.org/index.php/OWASP_favicon_database
* `curl <site> | md5sum`

### Sitemap.xml
* Gives permission for files owner wants to be searchable, can have vulnerabilities as well

### HTTP Headers
* Can tell us more information about the framework to make the website, use `curl <website> -v` to get more information

### Framework Stack
* We can read documentation websites to get more information to hack

## OSINT
* Open Source Intelligence

### Google Hacking/Dorking
* Uses google search engine (https://en.wikipedia.org/wiki/Google_hacking)
* site: - results in the site
* inurl - specific word in the url
* filetype - specific file exception
* intitle - specified word in title

### Wappalyzer
https://www.wappalyzer.com/ is a site that can tell you all information about a website

### Wayback Machine
* Historical archive of websites, can help uncover old active pages

### GitHub
* Can search github for more information

### S3 Buckets
* AWS storage buckets

## Automated Discovery
* Using tools to discover content rather than doing manually
* Uses wordlists

### Wordlists
* Common used words
* Great github repo is https://github.com/danielmiessler/SecLists

### ffuf, dirb, and gobuster
* These can all use word lists




