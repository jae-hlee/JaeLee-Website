---
layout: page
permalink: /building/
title: Building
description: Things I build outside the lab.
nav: true
nav_order: 5
---

Outside of research, I like to design and ship things end to end. Here are some projects I'm especially proud of.

## Actuator

<div class="actuator-figure">
  {% include figure.liquid loading="eager" path="assets/img/actuator.png" class="rounded z-depth-1" alt="Actuator: your AI can diagnose the problem, now it can hire someone to fix it" %}
</div>

**[Actuator](https://actuato.com)** is a marketplace where AI agents hire real people for real-world work. An assistant can diagnose the problem, but someone still has to turn the wrench. Actuator lets an agent post a structured job on behalf of the person it serves, lets vetted local workers bid with their own price and credentials, ranks the applicants for the person to choose from, and holds payment in escrow until the work is verified. It's live in Baltimore and expanding city by city.

The agent side is a full **OAuth 2.1** authorization server with a hosted **MCP** endpoint, so any assistant that supports remote MCP servers can connect once and then hire within a spending limit the person sets. Anything beyond that grant comes back as a pending approval for the person to sign off on. There's also a developer sandbox where five simulated workers bid, check in, upload evidence, and review on a short timer, so agent builders can exercise the whole lifecycle without real money moving.

It's a solo full-stack build: a **FastAPI** backend (async **SQLAlchemy**, **PostGIS** for worker coverage areas, **arq** for background jobs, **Stripe Connect** for escrow), a **Next.js** front end covering the landing site, consumer assistant, worker app, and admin, and matching **TypeScript** and **Python** SDKs generated from the OpenAPI schema. It runs on Vercel, Render, Neon, Upstash, and Cloudflare Workers.

[Visit actuato.com →](https://actuato.com) &nbsp;·&nbsp; [Connect your assistant →](https://actuato.com/connect-assistant)

## ScanDat

<div class="scandat-figure">
  {% include figure.liquid loading="eager" path="assets/img/scandat.png" class="rounded z-depth-1" alt="ScanDat AI: snap a flyer, get the event in your calendar" %}
</div>

**[ScanDat AI](https://scandat.app)** is an iOS and Apple Watch app I designed, built, and shipped to the App Store. Snap a photo of any flyer, poster, schedule, or screenshot (or paste text), and AI extracts the events and adds them straight to your **Apple or Google Calendar**.

It's a full-stack solo project: a native **Swift / SwiftUI** app (iPhone, Apple Watch, home-screen widgets, and a share extension) backed by a **FastAPI** service that proxies to a vision-language model for structured event extraction. It also handles Sign in with Apple and Google, StoreKit subscriptions, on-device auto-cropping and live text detection, and duplicate/conflict checks before anything reaches your calendar.

[Visit scandat.app →](https://scandat.app) &nbsp;·&nbsp; [Download on the App Store →](https://apps.apple.com/app/id6761404618)
