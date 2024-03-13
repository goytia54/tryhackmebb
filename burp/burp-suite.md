# BURP Suite
* Java based framework designed to serve as a comprhensive solution for conducting pen testing
* Industry standard, especially for APIs
* Captures and manipulates http/https traffic between browser and webserver

## Features of BURP
* Proxy: The Burp Proxy is the most renowned aspect of Burp Suite. It enables interception and modification of requests and responses while interacting with web applications.
* Repeater: Another well-known feature. Repeater allows for capturing, modifying, and resending the same request multiple times. This functionality is particularly useful when crafting 
payloads through trial and error (e.g., in SQLi - Structured Query Language Injection) or testing the functionality of an endpoint for vulnerabilities.
* Intruder: Despite rate limitations in Burp Suite Community, Intruder allows for spraying endpoints with requests. It is commonly utilized for brute-force attacks or fuzzing endpoints.
* Decoder: Decoder offers a valuable service for data transformation. It can decode captured information or encode payloads before sending them to the target. While alternative services exist for this purpose, leveraging Decoder within Burp Suite can be highly efficient.
* Comparer: As the name suggests, Comparer enables the comparison of two pieces of data at either the word or byte level. While not exclusive to Burp Suite, the ability to send potentially large data segments directly to a comparison tool with a single keyboard shortcut significantly accelerates the process.
* Sequencer: Sequencer is typically employed when assessing the randomness of tokens, such as session cookie values or other supposedly randomly generated data. If the algorithm used for generating these values lacks secure randomness, it can expose avenues for devastating attacks.

## BURP Dashboard
* Tasks: The Tasks menu allows you to define background tasks that Burp Suite will perform while you use the application. In Burp Suite Community, the default “Live Passive Crawl” task, which automatically logs the pages visited, is sufficient for our purposes in this module. Burp Suite Professional offers additional features like on-demand scans.
* Event log: The Event log provides information about the actions performed by Burp Suite, such as starting the proxy, as well as details about connections made through Burp.
* Issue Activity: This section is specific to Burp Suite Professional. It displays the vulnerabilities identified by the automated scanner, ranked by severity and filterable based on the certainty of the vulnerability.
* Advisory: The Advisory section provides more detailed information about the identified vulnerabilities, including references and suggested remediations. This information can be exported into a report. In Burp Suite Community, this section may not show any vulnerabilities.

## BURP Short Cuts
* Ctrl + Shift + D 	Dashboard
* Ctrl + Shift + T 	Target tab
* Ctrl + Shift + P 	Proxy tab
* Ctrl + Shift + I 	Intruder tab
* Ctrl + Shift + R 	Repeater tab

## Options
* Can set Global or Project Settings

## Intro to BURP Proxy
* Can intercept requests and held from reaching target server
* Capture and logging
* Websocket support
* Response interaction

### Proxy Settings
* Response Interception: Have to turn on
* Match and replace: allows regex to modify incoming and out going reqeusts

## FoxyProxy
* Firefox plugin to use to run proxy for burp suite
