---
title: "How to scale Alloy as a central telemetry gateway: capacity planning, load testing, and production lessons"
url: "https://grafana.com/blog/how-to-scale-alloy-as-a-central-telemetry-gateway-capacity-planning-load-testing-and-production-lessons/"
date: "2026-08-21"
author: "Fatjon Nebiu"
feed_url: "https://grafana.com/blog/index.xml"
---
Running Alloy as a single-instance sidecar is simple. Running it as a centralized gateway that absorbs the full telemetry stream of an enterprise platform—tens of millions of active series, terabytes of logs per day, and tens of thousands of trace spans per second—is a different challenge altogether. To get it right, you need deliberate capacity planning, honest load testing, and a monitoring setup that doesn't rely on the very thing you're testing.
