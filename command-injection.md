# Command Injection
* Abuse of an applications behavior to execute commands on the operation system using the same privileges that the apps uses to run
* Also known as remote code execution
* Top Ten OWASP

## Discovery
* Web apps pass data to and make a system call to machines OS
* This can often been in terms of an API endpoint

## Exploiting Command Injection
* Can use various shell operators to combine and execute commands
* Can be blind command injection
* Verbose command injection
* Can use `ping` and `sleep` commands
* cURL is a great way to test command injection

## Preventing Command Injections
* Input sanitation
* Bypassing Filters

## Comman injection payload list
