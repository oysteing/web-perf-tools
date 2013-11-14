===================

Apache Bench - simple CLI benchmark - Keep-Alive HTTP connection
```
ab -n 100 -c 20 -k http://www.example.org/
```

Siege - CLI benchmark
```
siege -c 20 -t 10S http://www.example.org/
```

Sproxy - discover all URLs of application
```
sproxy -o urls.txt
wget -r -o verbose.txt -l 0 -t 1 --spider -w l -e robots=on -e "http_proxy = http://127.0.0.1:9001" "http://www.example.org"
sort -u -o urls.txt urls.txt
```

JMeter

Blazemeter.com - cloud version of JMeter

Multi-mechanize - Python scripting for performance and load testing

beeswithmachineguns - fire up EC2 instances and run load tests
```
pip install beeswithmachineguns
bees up -s 2 -g default -z us-west-b1 -k ...
bees report
bees attack -n 100 -c 50 -u http://www.example.org
bees down
```

Google Page Speed API

WBench - client side timing
```
gem install wbench
wbench http://www.example.org
```
