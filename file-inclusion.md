# File Inclusion
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
