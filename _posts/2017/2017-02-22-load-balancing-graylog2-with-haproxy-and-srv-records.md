---
layout: "post"
title: "Load Balancing Graylog2 with HAProxy and SRV records"
date: "2017-02-22 12:40"
---

If you ever happen to use HAProxy to make load balance to your Graylog2/GELF inputs (you should try it, HAProxy is HAwesome!), I advice you to take a look to [Siaw Young's post][8517b56d].


As a plus, you may be using SRV record sets to maintain your Graylog2 cluster node list up to date.
If that applies to you, give it a try to [haproxy-srv][649f8b52].

Looking for a starting template for haproxy-srv? Here you have!

```
{{#dns-srv "_gelf._tcp.internal.example.org"}}
listen gelf :12201
    mode tcp
    balance roundrobin
    option httpchk GET /api/system/lbstatus
    {{#each this}}
        server gelf-{{@index}} {{ip}}:{{port}} check port 12900
    {{/each}}
{{/dns-srv}}
```

[8517b56d]: http://siawyoung.com/coding/sysadmin/graylog2/load-balancing-graylog-2-with-haproxy.html#change-haproxys-health-check-to-graylog2s-rest-api "Siaw Young's post"

[649f8b52]: https://github.com/elasticio/haproxy-srv/ "Flexible HAProxy auto configuration and auto service discovery for SkyDNS or Mesos-DNS"
