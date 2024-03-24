*** ABOUT THIS INFRASTRUCTURE:

* server: 
    computer hardware or software that give services to other computers, which are usually referred to as clients.

* The role of the domain name:
    To provide a human-friendly alias for an IP Address. The IP address and domain name alias is mapped in the Domain Name System (DNS)

* The type of DNS record www is in www.foobar.com.
    www.foobar.com uses an A record. This can be checked by running dig www.foobar.com.

* The role of the web server.
    accepts requests via HTTP or secure HTTP (HTTPS) and responds with the content of the requested resource or an error messsage.

* The role of the application server.
    host, install and operate applications and associated services for end users.

* The role of the database.
    maintain a collection of organized information that can easily be accessed, managed and updated

* What the server uses to communicate with the computer of the user requesting the website.
     the internet network through the TCP/IP protocol suite.

*** Issues With This Infrastructure

* In this infrastructure. there are multiple SPOF (Single Point Of Failure) 
For example, if the Application server is down, the entire processes would be down.

* Downtime when maintenance needed.
the website would be experiencing a downtime, if there is only one server.
in our case the server has to be turned off when we need to run some maintenance checks

* Cannot scale if there's too much incoming traffic.
 This server can quickly run out of resources or slow down when it starts receiving a lot of requests.
