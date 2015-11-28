



Graphite + statsd + carbon are running inside a docker 


Graphite : http://192.168.150.104:81/dashboard

Grafana :  http://192.168.150.104:3000/

NOTE : Grafana should ONLY be operated using CHROME browswer 


To populate graphite metric 
    while true; do   echo -n "example.statsd.counter.changed:$(((RANDOM % 10) + 1))|c" | nc -w 1 -u localhost 8125; done






