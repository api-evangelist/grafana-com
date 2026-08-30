---
title: "How volumetric sampling makes the most of your trace budget in Grafana Cloud"
url: "https://grafana.com/blog/how-volumetric-sampling-makes-the-most-of-your-trace-budget-in-grafana-cloud/"
date: "2026-08-13"
author: "Yuna Verheyden"
feed_url: "https://grafana.com/blog/index.xml"
---
Tracing is one of the richest observability signals, but it's also noisy and susceptible to data bloat. In a busy system, the vast majority of traces describe the same healthy, fast, successful request over and over, so most organizations downsample their traces to cut costs. But that approach has consequences, since the sampling strategy you choose determines whether you get a faithful picture of your whole system, or just a smaller, blurrier copy of your busiest endpoints.
