---
title: Eigth task
description: Draft
layout: layouts/post.njk
order: 9
tags: posts
---

> Which certificate authority issued the SSL certificate to the first domain from the previous question?

I right clicked on the packet from the first domain and followed the TCP stream. A little down in the response we can see `Go Daddy Secure Certificate Authority` repeated a lot.

![tcp stream godaddy certificate](/img/remote/cert-godaddy.PNG)

You can also use a DNS lookup service, type in the address and you'll get the same answer. Cool that it exists irl.

![dns lookup result](/img/remote/dns-lookup.PNG)