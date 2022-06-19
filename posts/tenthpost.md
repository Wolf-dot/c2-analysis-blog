---
title: Ninth task
description: Draft
layout: layouts/post.njk
order: 10
tags: posts
---

> What are the two IP addresses of the Cobalt Strike servers? Use VirusTotal (the Community tab) to confirm if IPs are identified as Cobalt Strike C2 servers. (answer format: enter the IP addresses in sequential order)

From the description on [Mitre](https://attack.mitre.org/software/S0154/):

    '[Cobalt Strike](https://www.cobaltstrike.com/) is a commercial, full-featured, remote access tool that bills itself as "adversary simulation software designed to execute targeted attacks and emulate the post-exploitation actions of advanced threat actors". Cobalt Strike’s interactive post-exploit capabilities cover the full range of ATT&CK tactics, all executed within a single, integrated system.'

We can also find the information that Cobalt Strike can communicate using HTTP, HTTPS and DNS.
We can find the IP addresses in the `Statistics > Conversations > TCP`, and now we have to look for those that fit the description.

[VirusTotal](https://www.virustotal.com) is a free analysis service for files and URL's for malicious content. We can input the IP address and see if it's been flagged.

![virus total result](/img/remote/virustotal.PNG)