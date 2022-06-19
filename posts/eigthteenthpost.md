---
title: Seventeenth task
description: Draft
layout: layouts/post.njk
order: 18
tags: posts
---

> The malware used an API to check for the IP address of the victim’s machine. What was the date and time when the DNS query for the IP check domain occurred? (answer format: yyyy-mm-dd hh:mm:ss UTC)

I filtered by the victim's IP address, DNS, and a keyword "api". The query: `ip.addr == 10.9.23.102 && dns && frame contains "api"`.