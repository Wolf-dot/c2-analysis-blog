---
title: Tenth task
description: Draft
layout: layouts/post.njk
order: 11
tags: posts
---

> What is the Host header for the first Cobalt Strike IP address from the previous question?

Get the ip address and look it up on the main search bar in WireShark: `ip addr == ***.***.**.***`.
Then select one of the packets and follow the TCP. The Host can be found on the second line.

![host header](/img/remote/host%20header.PNG)