# verfploeter-ttl-investigation
Explore the TTL values received from verfploeter anycast measurement tool


As part of SAND project [1], we have developed a tool to manage anycast catchment [2].
This tools provided a view of the catchments for each anycast node that we have.

In summary, the tool sends an ICMP request to each (/24) IPv4 over the Internet by using a anycast IP address as src IP.
Consequentelly, all the /24 will reply to the same anycast IP that will reach in different anycast node based on the routing.
The results provided by this tool can helps us to infer the node load, traffic distribution, and so on.

Recentelly, we are investigating the IP TTL from the packets that each anycast node receive. This projects aims to investigate 
the TTL distribution and explore anomalies in the value distribution.

[1] http://www.sand-project.nl/ <br>
[2] https://ant.isi.edu/software/verfploeter/index.html




![TTL clusters](https://github.com/joaoceron/verfploeter-ttl-investigation/blob/master/dataset/imgs/ttl.gif)
