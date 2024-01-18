# Content Discovery
* In this case we are not talking about obvious things to find
* Manually, Automated, OSINT (Open Source Intelligence)

## robots.txt
* Restricts what can't be searched, which could be valuable places to explore

## Favicon
* We can curl the favicon link and then run via `md5sum` to get a hash and search in https://wiki.owasp.org/index.php/OWASP_favicon_database
* `curl <site> | md5sum`
