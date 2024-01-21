# XSS
* Cross-Site Scripting
* Based on JavaScript
* Injection attack where malicious javascript gets injected into a web application

## XSS Payload
* JS code we want to execute on target computer
* Can use `alert` method to find entry points
  * `<script>alert('XSS');</script>`
 
## Reflected XSS
* HTTP request have data without any validation
* Can exist in parameters of query string
* URL File Path
* Sometimes HTTP Headers

![image](https://github.com/goytia54/tryhackmebb/assets/13384055/0aa8258d-1ec1-4bed-8597-2457deed3fb8)

## Stored XSS
* Stored on the web application, blog post which allows people to post comments

![image](https://github.com/goytia54/tryhackmebb/assets/13384055/c2e99943-b2e4-49c9-91c2-be5b35f78ae8)

## DOM Based XSS
* Document Object Model, programming interface between HTML and XML

![image](https://github.com/goytia54/tryhackmebb/assets/13384055/374caf25-696c-4e53-b455-05dc421717f2)

## Blind XSS
* Similar to stored, but can't test against yourself
* Example: Sending a xss into a contact form and then it sends information back to an attacker
* https://github.com/mandatoryprogrammer/xsshunter-express can be used for blind XSS diagnosis.



