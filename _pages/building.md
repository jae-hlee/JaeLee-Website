---
layout: page
permalink: /building/
title: Building
description: Things I build outside the lab.
nav: true
nav_order: 5
---

Outside of research, I like to design and ship things end to end. Here are some projects I'm especially proud of.

## ScanDat

<div class="scandat-figure">
  {% include figure.liquid loading="eager" path="assets/img/scandat.png" class="rounded z-depth-1" alt="ScanDat AI: snap a flyer, get the event in your calendar" %}
</div>

**[ScanDat AI](https://scandat.app)** is an iOS and Apple Watch app I designed, built, and shipped to the App Store. Snap a photo of any flyer, poster, schedule, or screenshot (or paste text), and AI extracts the events and adds them straight to your **Apple or Google Calendar**.

It's a full-stack solo project: a native **Swift / SwiftUI** app (iPhone, Apple Watch, home-screen widgets, and a share extension) backed by a **FastAPI** service that proxies to a vision-language model for structured event extraction. It also handles Sign in with Apple and Google, StoreKit subscriptions, on-device auto-cropping and live text detection, and duplicate/conflict checks before anything reaches your calendar.

[Visit scandat.app →](https://scandat.app) &nbsp;·&nbsp; [Download on the App Store →](https://apps.apple.com/app/id6761404618)
