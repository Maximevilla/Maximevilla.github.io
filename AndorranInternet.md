---
title: Andorran Internet - LookLike
date: 2018-07-18 14:00:00
---

### How Looks the Andorra on the Internet ?

First, let's take the Andorran netRange and put it on the entire IPv4 range. For that we will use the Hilbert curve. For that I've used the tool from this repo https://github.com/measurement-factory/ipv4-heatmap.

> I advice you, you'll need to zoom! 
>


![](/img/AndorraInInternet.png)

> As we can see, Andorra could been easyly forgotten from anyone who doesn't look closer...
>

#### And the Andorran CIDR Scope ? 

Let's have a look at it.

* After having scanned the 40 000 IPs. we can then have a look at what we get. 

>Let's first have a look at the used address space.
>

![](/img/VRE-AddressSpace.svg)

* and with the ports ?

![](/img/IVRE-IPsPorts.svg)


This tells nothing special to us. But we already know that only 10 % of the IPRange responds to a ping. Although, there are some no responding hosts ith open ports. 

We could dive further, trying to check how many hosts use certificates. How many don't already use only https for example.What are the services exposed.

> Last year I found more than 100 rdp into the wild. This year they are only 6. **Keep Watching, Things get Better**
>
        
