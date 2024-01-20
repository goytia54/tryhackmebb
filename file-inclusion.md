![image](https://github.com/goytia54/tryhackmebb/assets/13384055/7b904686-234c-49a1-9d86-70de298c478a)# File Inclusion
* Being able to access files/directories we shouldn't be able too

## Path Traversal
* Also know as directory traversal, allows us to read OS resources such as local files on server running application
* The endpoint is not the problem however poor input validation or filtering is cause
* `dot-dot-slash` attack `../`
```
/etc/issue
	contains a message or system identification to be printed before the login prompt.
/etc/profile
  controls system-wide default variables, such as Export variables, File creation mask (umask), Terminal types, Mail messages to indicate when new mail has arrived
/proc/version
	specifies the version of the Linux kernel
/etc/passwd
	has all registered user that has access to a system
/etc/shadow
	contains information about the system's users' passwords
/root/.bash_history
  contains the history commands for root user
/var/log/dmessage
	contains global system messages, including the messages that are logged during system startup
/var/mail/root
  all emails for root user
/root/.ssh/id_rsa
	Private SSH keys for a root or any known valid user on the server
/var/log/apache2/access.log
  the accessed requests for Apache  webserver
C:\boot.ini
	contains the boot options for computers with BIOS firmware
```
## LFI
* Local File Inclusion
* Some php functions such as `include` which gives us access to other files
* Can use null bytes to inject to remove filtering out
* Can use `.` as well to help filter
* Might have to use the actual directory in the file as well

## RFI
* Remote file inclusion
* Could get remote conmmand execution
* Sensitive Information Disclosure
* Cross-site scripting (XSS)
* Denial of Service (Dos)

![image](https://github.com/goytia54/tryhackmebb/assets/13384055/0122705b-7e57-4f64-b0e9-986a63fbdd22)

## Developer Suggestions
* Keep system and services, including web application frameworks, updated with the latest version.
* Turn off PHP errors to avoid leaking the path of the application and other potentially revealing information.
* A Web Application Firewall (WAF) is a good option to help mitigate web application attacks.
* Disable some PHP features that cause file inclusion vulnerabilities if your web app doesn't need them, such as allow_url_fopen on and allow_url_include.
* Carefully analyze the web application and allow only protocols and PHP wrappers that are in need.
* Never trust user input, and make sure to implement proper input validation against file inclusion.
* Implement whitelisting for file names and locations as well as blacklisting.
