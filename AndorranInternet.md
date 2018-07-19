---
title: Andorran Internet
date: 2018-07-18 14:00:00
---

### How Looks Andorra on the Internet ?

First, let's take the Andorran NetRange and put it on the entire IPv4 range. We will use the [Hilbert curve](https://en.wikipedia.org/wiki/Hilbert_curve). For that I've used the tool from this repo [https://github.com/measurement-factory/ipv4-heatmap](https://github.com/measurement-factory/ipv4-heatmap).

> I advice you, you'll need to zoom! 
>


![](/img/AndorraInInternet.png)

> As we can see, Andorra could been easyly forgotten from anyone who doesn't look closer...
>

#### And the Andorran CIDR Scope ? 

Let's have a look at it.

* After having scanned the 40 000 IPs. we can then have a look at what we get. 

> As a starter we notice that only 10 % respond to a ping.
>

![](/img/IVRE-AddressSpace.jpeg)

* And with the ports ?

![](/img/IVRE-IPsPorts.jpeg)


We already know that only 10 % of the IPRange responds to a ping. Although, there are some no responding hosts with open ports. 

We could dive further, trying to check how many hosts use certificates. How many already use only https. Or, what are the services exposed ?

## Just a look ! I promise...

For that you could probably start to search [there](https://www.shodan.io/report/Ox9MLkNM). Looking at that report, one of the things that blinks to us is that an optician with one shop has 3564 hosts up. That's for sure something that deserves some investigation. So let's have a look.

We type in shodan :

~~~~
country:ad org:"Guineu Optica Companyia SL"
~~~~

As a result we get :

| Owner |Andorra | Guineu Optica Companyia SL
| ------------- |:-------------:| -----:|
| Qty | 24,352 | 3,564 |




| Top Services | SNMP | SMTP |
| ------------- |:-------------:| -----:|
| Qty |1,869 | 1,695 |


That's weird. An optician running almost 2000 SNMP and SMTP... We could maybe, ... No.

For full shodan report, [click](https://www.shodan.io/report/Sc7240bf).

> Last year I found more than 100 rdp into the wild. This year they are only 6. **Keep Watching, Things get Better**
>
        
