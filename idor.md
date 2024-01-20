# IDOR
* Insecure Direct Object Reference
* Access Control Vulnerability

## IDOR example
* Being able to change values in query strings to access data you should be able to

## IDOR Encoding
* Some data can be encoded, base64 is common

## IDOR Hash Ids
* Some data can be hashed as well, crackstation.net can help with that as well, such as md5 hash

## IDOR in upredicable IDs
* If can't crack it, make two accounts and try swapping ids

## IDOR Locations
* Could be in URL
* Can use parameter mining to find other query strings for a valid url
* Can also be in json or loaded through AJAX
