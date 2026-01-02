# Linux Escalations 

## Kernal Exploits
Using `exploit-db` to find kernal exploits after enumration

## Sudo
* Using something like the gtfobins.github.com to find problems

## SUID
* `find / -type f -perm -04000 -ls 2>/dev/null` to find programs that can be run without needing sudo expose information (`nano` or `base64` for example)
