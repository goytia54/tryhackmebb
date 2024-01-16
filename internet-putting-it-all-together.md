# Putting It All Together
* Request -> DNS -> View Website -> Connect To Web Server

## Other Components

### Load balancers
* could be round robin or weighted
* have health checks and will stop traffic until health check works again

### CDN
* Content Delivery Network
* Host files like images and videos

### Dtabases
* Things like mysql, oracle, mongo, graphql

### WAF
* Web Application Firewall
* Sits between web request and web server, protect against hacking or denial of service attacks
* Checks for certain attacks

## Web Servers
*  Software that listens to incoming connections
*  Web server delivers files

## Virtual Hosts
* text base configuration files

## Static Versus Dynamic Content

## Request Order
Request -> Local IP Cache Check -> ISP IP Cache Check -> Intenet IP Cache Check -> Authoritative DNS -> WAF -> Load balancer -> Connect to web  server -> HTTP Request -> Web application -> Serve HTML

![Screen Shot 2024-01-15 at 9 03 59 PM](https://github.com/goytia54/tryhackmebb/assets/13384055/dbe51105-8e1b-467b-8d10-420276fe17ac)
