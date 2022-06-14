---
title: Seventh task
description: Draft
layout: layouts/post.njk
order: 8
tags: posts
---

> Malicious files were downloaded to the victim host from multiple domains. What were the three domains involved with this activity?

Here I had to use a hint, which told me to filter the search down to HTTPS traffic. I did so, `ip.addr == 10.9.23.102 && tcp.port == 443` and ordered them by the size of the packets.
But to see the domain names we have to enable them, so I went into `View > Name Resolution > Resolve Network Addresses`. Now a little scrolling and I got the three that fit the answer format.

![malicious hosts](/img/remote/malicious-hosts.PNG)