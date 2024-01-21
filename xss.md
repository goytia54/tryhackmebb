# XXS
* Cross-Site Scripting
* Based on JavaScript
* Injection attack where malicious javascript gets injected into a web application

## XXS Payload
* JS code we want to execute on target computer
* Can use `alert` method to find entry points
  * `<script>alert('XSS');</script>`
 
## Reflected XSS
* HTTP request have data without any validation
* Can exist in parameters of query string
* URL File Path
* Sometimes HTTP Headers

![image](https://github.com/goytia54/tryhackmebb/assets/13384055/0aa8258d-1ec1-4bed-8597-2457deed3fb8)
