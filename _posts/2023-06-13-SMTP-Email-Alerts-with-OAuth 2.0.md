---
title: SMTP Email Alerts with OAuth 2.0
---
## Why would one use email alerts?
The reason one would use email alerts is because day to day operations at a company can sometimes get so hectic that it can be difficult to sometimes spare a minute to be able to sufficiently check things. Products like ticketing systems and backup systems often come with these services as a feature. One way of setting up alerts securely would be to utilize OAUth2.0 authorization/authentication to utilize SMTP services. 

## How to set these services up
Exact instructions differ from product to product - however some steps tend to be the same.
Firstly, one needs to use platforms such as Google's platform or Microsoft 365 to properly configure such services. Google has free API service in the console that can be used to set up OAuth screening. However, before any of that, you need to specify the SMTP
server you would want to use. The following is the information you would probably fill in/utilize for the Gmail SMTP server most accounts would use. Take note - that there are two ports you can use, each utilizing a different network communication protocol,
I would suggest using the TLS one because it is more secure and uses newer technology than the SSL one. 

* Gmail SMTP server address: smtp.gmail.com
* Gmail SMTP username: Your full Gmail address (e.g. you@gmail.com)
* Gmail SMTP password: The password that you use to log in to Gmail
* Gmail SMTP port (TLS): 587
* Gmail SMTP port (SSL): 465

Two products you can do this with are OSTicket and Vaaem for example. 
