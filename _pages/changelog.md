---
layout: page
title: What's New
include_in_header: true
---

# Changelog
The highlights below track public milestones for the Your Golf Coach beta. For technical implementation details refer to the TASK documents in the main source repository.

<br>

### `Latest`
# **Version 0.9.0 — Public TestFlight Beta**
**Released:** November 2024

#### What's New
- Added privacy-compliant Terms & Privacy screens with consent controls.
- Refined Launch Monitor gating and telemetry for more reliable impact detection.
- Updated Academy tab with Fabian Bünker branding and external links.
- Finalized localization for English and German, including legal copy.

#### Fixes & Improvements
- Offline sync banner now shows queued changes count.
- Additional analytics events for trend cards and launch-monitor states.
- Reduced cache churn for launch-monitor footage (FIFO, 30-day TTL).

<br>

### **Version 0.8.0 — Feature Complete Build**
**Released:** October 2024

#### What's New
- Scorecard overhaul with expectationless rating sliders.
- Trend dashboard with strokes, putts, and category spark lines (last 10 holes).
- Offline mode with sync queue, reachability service, and user messaging.
- Apple Watch rhythm companion with shared haptic cadence.

#### Fixes & Improvements
- Added Firebase Analytics + Crashlytics opt-in layer.
- Hardened CloudKit conflict resolution and retry logic.

<br>

### **Version 0.7.0 — Rhythm + Scorecard Alpha**
**Released:** September 2024

#### What's New
- Initial SwiftUI tab structure (Home, Training, Academy, Statistics, Info).
- Rhythm Trainer MVP (1-2-3-4 cadence, audio + haptics).
- Classic scorecard entry with Core Data persistence.

#### Fixes & Improvements
- Brand color system (#083147 / #fa7921) applied across typography and controls.
- Integrated localization scaffolding and in-app support links.

<br>

Need the historical TestFlight notes? Email [app@fabianbuenker.de](mailto:app@fabianbuenker.de) and we can provide prior builds or more detailed QA logs.
