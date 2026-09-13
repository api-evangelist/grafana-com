---
title: "Custom labels in Grafana Cloud Synthetic Monitoring: New updates for consistency and ease-of-use"
url: "https://grafana.com/blog/synthetic-monitoring-labels-update/"
date: "2026-09-10"
author: "Anant Sharma"
feed_url: "https://grafana.com/blog/index.xml"
---
Labels are a powerful way to organize telemetry and define policies across Grafana Cloud, helping to streamline alerting, attribution, access control, and more. But traditionally, custom labels in Synthetic Monitoring have worked a little differently: they only lived on a single sm_check_info metric, and Grafana Cloud prefixed each one with label_ . To make custom labels in Synthetic Monitoring work consistently with the rest of Grafana Cloud—without extra joins, naming conventions, or workarounds—we're rolling out an update that lets your custom labels attach directly to every check metric, n
