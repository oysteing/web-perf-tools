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
