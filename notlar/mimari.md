---
layout: default
title: "Çerez notlar"
---

# AdTech Mimari Akışlar

## 📖 Genel Bakış

```text
                ┌────────────────────────────┐
                │        ADVERTISER          │
                │  Brands / Agencies / SMEs  │
                └────────────┬───────────────┘
                             │  Campaign Setup via UI / API
                             ▼
┌────────────────────────────┴────────────────────────────┐
│                DEMAND-SIDE PLATFORM (DSP)               │
│  • Campaign Management (UI/API)                         │
│  • Bidding Engine (RTB)                                 │
│  • Budget, Targeting, Frequency Capping                 │
│  • Uses DMP Data (1st/2nd/3rd Party Segments)           │
└────────────┬──────────────────────┬─────────────────────┘
             │                      │
             │ Bid Requests          │ Audience Sync / Data Fetch
             ▼                      ▼
┌────────────────────────────┐   ┌────────────────────────────┐
│         AD EXCHANGE        │   │     DATA MANAGEMENT        │
│  • OpenRTB Auction Layer   │   │         PLATFORM (DMP)     │
│  • Real-Time Matching      │   │  • Data Collection (Tags,  │
│  • Fraud/Viewability API   │   │     APIs, Cookies, SDKs)   │
│                            │   │  • Data Normalization &    │
│                            │   │     Enrichment             │
│                            │   │  • Audience Segmentation   │
│                            │   │  • Activation (to DSP/SSP) │
└────────────┬───────────────┘   └──────────────┬────────────┘
             │                                  │
             │ Winning Bid / Impression Event    │ Audience Matching / Enrichment
             ▼                                  ▼
┌────────────────────────────┐   ┌────────────────────────────┐
│     SUPPLY-SIDE PLATFORM   │   │        AD SERVER           │
│  • Publisher Inventory Mgmt│   │  • Ad Delivery & Tracking  │
│  • Header Bidding          │   │  • Impression / Click Logs │
│  • Yield Optimization      │   │  • Conversion Tracking     │
└────────────┬───────────────┘   └──────────────┬────────────┘
             │                                  │
             │ Ad Display / Event Tracking       │ Event Log Sync
             ▼                                  ▼
┌────────────────────────────┐   ┌────────────────────────────┐
│        PUBLISHER           │   │   ATTRIBUTION SERVICE      │
│  • Web/App SDK             │   │  • Impression→Click→Conv.  │
│  • Ad Slots                │   │  • Multi-Touch Models      │
│  • Consent Mgmt (CMP)      │   │  • Cross-Device Matching   │
└────────────────────────────┘   └────────────────────────────┘
```