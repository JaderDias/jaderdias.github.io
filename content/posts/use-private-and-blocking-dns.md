---
title: "Protect your privacy and security with private and blocking DNS"
date: 2022-02-17T20:00:00+01:00
draft: false
---
When you're online on your smartphone, laptop, smart TV, or even when you simply have a WiFi lightbulb, there are many ways your Internet Service Provider (ISP), governments, companies and other can track your activities and display ads.

The first step towards privacy is to stop using your internet provider's DNS service and use an encrypted one. DNS over HTTPS (DoH) and DNS over TLS (DoT) are forms of encryption provided by Google DNS, Cloudflare DNS, among others. This prevents your ISP and possible other men-in-the-middle (MITM) from sniffing into your name resolution request. The main difference between DoH and DoT is that the former looks like normal HTTPS traffic, and it's harder for government and ISPs to prevent you from using it, if you're in a very strict environment. The latter, DoT, is theoretically faster. Android allows you to configure a Private DNS easily, while on iOS you need to load a special file, called profile, to be able to use it. While it can also be used in laptops and desktops, the only way to use it in TVs, lamps, switches, cameras is to have a prosumer router or a PiHole.

A PiHole will help you more than just give you private. The routers given to us by our ISPs are terrible at performing all of the multiple functions they have: modem, router, switch, firewall and WiFi access point. Having a small form computer, like a Raspberry Pi, in your network allows you to complement the capabilities of your home router. Installing PiHole on a Raspberry Pi allows you to give not only private DNS service to all devices in your network, but also allows you to block ads, tracking, malware and phising.

But what about when you step out of the house? You could expose your home's PiHole via Dynamic DNS (DDNS), or get a fixed IP from your ISP, but there are similar services that you could use both inside and outside your home network, namely AdGuard DNS and NextDNS. They would still need DDNS or a PiHole to work with Smart devices that aren't as configurable as a Smartphone, but they should be more available than your home network.