---
title: "A new allowlists design for Grafana Cloud IP addresses: What you need to know"
url: "https://grafana.com/blog/a-new-allowlists-design-for-grafana-cloud-ip-addresses-what-you-need-to-know/"
date: "2026-07-23"
author: "Pablo Angulo"
feed_url: "https://grafana.com/blog/index.xml"
---
If your network restricts inbound or outbound traffic, you likely maintain an allowlist of Grafana Cloud IP addresses so your systems and Grafana Cloud can talk to each other. Today we're introducing a new allowlists design : a single, structured API that replaces the collection of per-product lists we've published until now. If you don't use IP allowlisting—or you connect to Grafana Cloud over private connectivity such as AWS PrivateLink—nothing changes for you, and no action is needed.
