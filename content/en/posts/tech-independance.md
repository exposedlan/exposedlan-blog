+++
date = '2025-01-09T01:04:19+01:00'
draft = true
title = 'Privacy & Tech independance'
tags = ['Technology', 'Privacy']
+++

## Why ?
Everyday we let big companies like *Google*, *Meta*, *X*, *Reddit*, etc, watch and remember slices of our lifes, and often sensitive parts of it that you shouldn't share publicly.
We trust people that we don't know, giving them our sensitive data, all of it is on another's person computer after all.
<br>Hundreds of cases of personal data leaks happened, companies keep getting hacked and critical informations as social security numbers, names, address, etc.. keeps leaking to the public, and it still happening to this day.<br>

What percentage of you digital life is on your own devices? Lot of people rely (almost) exclusively on 3rd party services and I find it scary.

<br>
If you're interested by the subject, I recently came across this really cool pdf by *Psychcool* :
<br><sub><sup>(sadly he seems to have deleted almost all of his accounts, I hope he's doing well)</sub></sup>

{{< pdfReader "/docs/Spyware.pdf" >}}

## Don't fall for the VPN trap
For some years now, we saw an explosion in VPN ads, claiming to improve privacy, letting you hide your real IP and access geo-blocked content.

One of the big selling point VPN companies are trying to sell you, is improved privacy and security on (public) networks, thanks to an amazing encrypted tunnel!
<br>
See, if you don't know how HTTP(S) works, the little lock next to the URL in your browser indicate that you're using the **HTTPS protocol.** It means that all the traffic exchanged between you and the website is going through an encrypted tunnel, it's been more than a decade since almost all websites uses HTTPS by default. Furthermore, **every iOS apps since 2016** and every **Android apps from 2018** uses HTTPS 

![HTTPS-enabled website](/screenshots/https-website.webp)

Yes, an encrypted tunnel, just like a VPN. And if someone tried to attack you with [Arp Spoofing](https://wikipedia.org/wiki/ARP_poisoning), **It won't work.**

![Browser error related to wrong SSL certificate](/screenshots/connection-not-private.webp)

They also *really* like to use the **"Miltary-Grade Encryption"** argument, it refers to **AES** (Advanced Encryption Standard) which is used LITERALLY everywhere. (you're using it to read this post), so it's not very special.

It is true that your ISP / Country can see what base domains (and ONLY base domains) you visited, it **can not see on which pages you went nor the content of it.** VPN ads tend to imply the opposite to scare people.
<br>
It can effectively hide some of your browsing habits and protocol used from your ISP, and it can be useful in certain Countries that are heavily censored, but **don't fall into thinking that you ISP / Country can see everything you do on the Internet.** However, like I said before, it can improve your privacy to a certain extent.

I believe that **a lot of people using VPNs don't really need them,** the only use cases I see for *'normies'* is **accessing geo restricted content** or **bypassing censor.** If you bought a VPN thinking it will improve your security while browsing the Internet, it may be time to save a few bucks per month.

Finally let's get to the meat and potatoes. When you're using a VPN, all your traffic goes back and forth through VPN's servers. Essentially, you trust someone's PC to pass-through all of your traffic. This person might have said to you *"I promise I won't look at your data!"* or *"I don't have any decryption key"*, **you never went to their office to verify these claims.** They probably already have your name, email adress, credit card details, or any information related to you, so **they know who you are**.<br>
It also applies to VPN providers who claims to not log your activities, **you can't be sure.** Many, many of providers showed that they work with authorities when necessary (then they probably have some sort of logs)
<br>
Why your ISP would spy on you, and this company that you didn't know before wouldn't? **Selling data to advertisers is the main source of income for a lot of companies.**
<br>

And this logic applies to every Tech Company. It's not because an company is well-known or is making appealing claims that you should trust it, it's ALWAYS someone else's computer and **you DON'T know** what they're really doing **unless it's open-source.**
<br>

This is why, if you need a VPN, I recommend [Mullvad](https://mullvad.net), It does not require ANY personal information at signup and you can even pay in cash! <sub><sup>(not an ad)</sub></sup> It just gives you an unique number, no password, no nothing. Therefore, even if some of your traffic could be logged, they won't know anything about who is behind the account (except your IP).

*source: [Tom Scott's video](https://www.youtube.com/watch?v=WVDQEoe6ZWY) and personal knowledge about networks and VPNs*
## Moving away from 3rd party services
If you have any spare computer at home, you can install an Linux distribution on it and start hosting your own services. You can find a lot of [tutorials for Docker](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04) on the Internet, and for beginners, I recommend [Portainer](https://docs.portainer.io/start/install-ce) to manage containers with a nice graphical interface.
I'll write a detailed guide to setup a personnal server in another post.

Here's some alternative to popular apps/services that you can self-host yourself:

| App/Service | Alternative      |
| --------  | ----------------- |
| Google | SearXNG |
| Google Drive | Nextcloud |
| Google Docs | Collabora Office / ONLYOffice (paired with Nextcloud) |
| Google Analytics | Umami / Matomo
| Netflix (and other streaming services) | Jellyfin|
| Spotify (and other music services)| PlexAmp / Airsonic-advanced |
| Notion | SiYuan Notes / Focalboard |
| Notes | Joplin |
| Discord   | Matrix (via Element)  |
| Slack     | Mattermost        |
| Airdrop | Pairdrop |
| AnyDesk | RustDesk |
| Youtube   | Peertube or Invidious |
| Reddit    | Lemmy             |
| Zoom      | Jitsy             |
| Cooking recipes | Mealie / Tandoor |

Note that a lot of them doesn't need self-hosting to be used. They sometimes offer to use the service on known instances hosted by other people themselves. (like [Invidious](https://invidious.io/), [Matrix](https://servers.joinmatrix.org/) or [SearXNG](https://searx.space/))

## Basic tips for privacy

First, **don't use Chrome nor any chromium based browsers**, use **firefox / brave or browsers based on them**, then start using adblockers like [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin) which supports **custom blocklists** by the way, it means that you can block pretty much everything you want (trackers, gambling, pron, specific social networks, etc..)<br>
Next, try to **stop using Cloud** services, or use them **as little as possible**. Your own data should be on your own hardware.

<br>Use better privacy-focused apps/services for your social networks and messaging needs.
Here's some alternatives to your prefered websites: <sub><sup>(I know most of them where already shown above)</sub></sup>

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
