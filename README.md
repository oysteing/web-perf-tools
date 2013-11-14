===================

Apache Bench - simple benchmark - Keep-Alive HTTP connection
```
ab -n 100 -c 20 -k http://www.example.org/
```

Siege - command-line benchmark - 100 requests with 20 threads Keep-Alive
```
siege -c 20 -t 10S http://www.example.org/
```
