# SSRF
* Server Side Request Forgery
* Allows user to cause the webserver to make additional or editited HTTP request to resource of choosing

## Successful SSRF
* Access to unauthorized areas
* Access to customer/org data
* Ability to scaled to internal networks
* Reveal auth tokens and creds
* can be regular (info returned) and blind (occurs but no info returned)

## We can target URLs 
* Example 1:
![image](https://github.com/goytia54/tryhackmebb/assets/13384055/f24e4e28-f60a-4301-bef0-45f5d5571dc0)
Example 2:
![image](https://github.com/goytia54/tryhackmebb/assets/13384055/9ad44261-f59c-4cc9-96fa-ae75de830b69)
Example 3:
![image](https://github.com/goytia54/tryhackmebb/assets/13384055/b0c67481-3671-4e1c-b948-923974243491)
Example 4:
![image](https://github.com/goytia54/tryhackmebb/assets/13384055/cb3cfc78-2db4-4c34-bf44-890d1114d854)

## Finding an SSRF
* When a full URL is used in a parameter in the address bar:
* A hidden field in a form:
* A partial URL such as just the hostname:
* Or perhaps only the path of the URL:
* Can use requestbin.com to monitor HTTP requests
