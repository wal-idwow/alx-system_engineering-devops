*** For this infrastructure

* For every additional element:
    the load balancer: The HAProxy load balancer is configured with the Round Robin distribution algorithm. This algorithm works by using each server behind the load balancer in turns, according to their weights.

* distribution algorithm the load balancer is configured with and how it works:
    processing time stays equally distributed. As a dynamic algorithm
    allows server weights to be adjusted on the go.

* load-balancer enabling an Active-Active or Active-Passive setup, explain the difference between both:
    The HAProxy load-balancer is enabling an Active-Passive setup.
    - Difference:
        Active-Active setup: the load balancer distributes workloads across all nodes in order to prevent any single node from getting overloaded.
        Active-Passive setup: the load balancer distributes worloads accross only one node that must be active

* How a database Primary-Replica (Master-Slave) cluster works:
    primary database(Master):
        - source for read and write operations
        - all operations performed
    replica database(slave)
        - receive and apply changes from the primary DB
        - serve read-only queries
        - used for backups, analytics, reporting

* The difference between the Primary node and the Replica node in regard to the application.
    The Primary node: is take all the write operations the site needs.
    the Replica node: is capable of processing read operations, which decreases the read traffic to the Primary node.

*** Issues With This Infrastructure


* there are multiple SPOF (Single Point Of Failure) 
For example, if the Application server is down, the entire processes would be down.

* Security issues.
The data transmitted over the network isn't encrypted using an SSL certificate so there is no safety. There is no way of blocking unauthorized IPs also there's no firewall installed

* No monitoring.
We can't knowing the status of each server since they're not being monitored.