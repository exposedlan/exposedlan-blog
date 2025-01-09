+++
date = '2025-01-09T01:04:19+01:00'
draft = true
title = 'Tech Independance'
+++

## Why ?
Everyday we let big companies like *Google*, *Meta*, *X*, *Reddit*, etc, watch and remember parts of our lifes, and often sensitive parts that you shouldn't share with others.<br>
We trust people that we don't know, giving them our sensitive data, all of it is on another's person computer. Hundreds of cases happenned, companies keep getting hacked and critical informations as social security numbers, names, address, etc.. keeps leaking to the public, and it still happening to this day.<br><br>
If you're interested by the subject, I recently came across this really cool pdf by *Psychcool* :
<br><sub><sup>(sadly he seems to have deleted almost all of his accounts, I hope he's doing well)</sub></sup>

{{< pdfReader "/Spyware.pdf" >}}

## Ok, how do I resolve this issue ? (basic)

First, **don't use Chrome nor any chromium based browsers**, use **firefox or firefox based browsers**, then start using adblockers like [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin) which supports **custom blocklists**, it means that you can block pretty much everything you want (trackers, gambling, pron, specific social networks, etc..)<br>
Next, try to **stop using Cloud** services, or use them **as little as possible**. Your own data should be on your own hardware.

<br>Use better privacy-focused apps/services for your social networks and messaging needs.
Here's some alternatives to your prefered websites:

| Most known | Alternative      |
| --------  | ----------------- |
| Messaging | Signal            |
| Discord   | Matrix (via Element)  |
| Slack     | Mattermost        |
| Youtube   | Peertube or Invidious |
| Reddit    | Lemmy             |
| Zoom      | Jitsy             |

Avoid smart home devices, they often are **poorly secured**, some are **very intrusive** and they **collect A LOT of data**. if you're interested in the poor security of IoT devices, check out [Matt Brown's videos](https://www.youtube.com/@mattbrwn).<br>
If you really want smart devices, I recommend putting them in a **separate VLAN** or in an **isolated network**. If not possible, you can also **setup a DNS sinkhole** like [Pi-Hole](https://pi-hole.net/) or [Adguard Home](https://adguard.com/adguard-home/overview.html) to **block most of telemetry** requests **on a network level**.
