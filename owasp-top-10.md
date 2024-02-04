# OWASP Top Ten
1. Broken Access Control
2. Cryptographic Failures
3. Injection
4. Insecure Design
5. Security Misconfiguration
6. Vulnerable and Outdated Components
7. Identification and Authentication Failures
8. Software and Data Integrity Failures
9. Security Logging & Monitoring Failures
10. Server-Side Request Forgery (SSRF)

## Broken Access Control
* If everyday user can access a page they are able to, then broken access control
* Allows users to bypass authorisation, view sensitive information or perform task they aren't suppose to

### IDOR
* Insecure Direct Object Reference: access resources you normally should not be able to see
* Object means something like a file, user, or anything you shouldn't be able to see without proper authorization
* Bascially being able to change endpoints as so `/object=1` can also access `/object=2` 

## Cryptographic Failures
* Vulnerability arising from the misue or lack of use cryptogrpahic algos to protect sensitive information
* Man in the middle attacks can occur where a hacker directs to there application so they can gather encrypted information to try and decrypt lady

### Databases
* Most common place to store data, using SQL
* Databases can also be stored as a files

#### Flat File Database
* `sqlite3` command for SQLite database
* `sqlite3 <db>` to access
* `.tables`

### Kali Linux
