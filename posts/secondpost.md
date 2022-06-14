---
title: First task
description: Draft
date: 2021-06-29
scheduled: 2021-06-29
layout: layouts/post.njk
order: 2
tags:
    - posts
---

> What was the date and time for the first HTTP connection to the malicious IP?
> (answer format: yyyy-mm-dd hh:mm:ss)

When we first open the capture file we can see a lot of packets.
I decided to order them by size and pick the IP address that had the showed the biggest packets. The one that stood out was `10.9.23.102`.
Then I filtered them by that IP with `ip.addr == 10.9.23.102`. The date format doesn't fit the one needed for the answer so I changed that in `View > Time Display Format > Date and Time of Day`. We need the first HTTP connection so I changed the filter to `ip.addr == 10.9.23.102 && http`.
Now we can see the first connection came at `2021-09-24 16:44:38`.

![first connection](/img/remote/first-date.PNG)