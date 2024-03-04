# SQL Injection
* Structured Query Language

## SQL Injection
* When a web app using SQL can be injected with SQL
* We can add comment lines such as `;--`

## In-Band SQLi
* Easiet to detect and exploit
* Discovering vulnerability and being able to extract data

### Error Based SQLi
* Useful obtaining information about the database strucuture as error messages printed to screen

### Union-Based SQLi
* Uses union operator with a select to return additional information

## Blind SQLi
* Unlike In-Band, we can't see the results of our attack directly on screen

### Authentication Bypass
* getting pass the login

### Boolean Based
* result received back is boolean based
* trying to see what options make the query selection true, say if a username already exits 

### Time Based
* Using a sleep to try to get system to sleep

## Out-of-Band SQLi
* Having two communication channels, one to launch attack and other to gather results.

### Steps
1) An attacker makes a request to a website vulnerable to SQL Injection with an injection payload.
2) The Website makes an SQL query to the database which also passes the hacker's payload.
3) The payload contains a request which forces an HTTP request back to the hacker's machine containing data from the database.

![image](https://github.com/goytia54/tryhackmebb/assets/13384055/b8d23987-a1f2-421a-add3-ca5b7203bbad)

### Remediation
* Prepared statements ensuring code does not change
* Input validation
* Escaping user input

## Helpful Commands
* `' OR 1=1--`, where the `OR 1=1` will always evaulate a prior statment to true and the `--` comments out the remaing statements
