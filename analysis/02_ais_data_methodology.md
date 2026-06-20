# AIS Data Methodology: Open-Source Maritime Intelligence

## Overview

Automatic Identification System (AIS) is a tracking technology mandated by the International Maritime Organization (IMO) for most vessels over 300 gross tonnage on international voyages (with lower thresholds for passenger vessels). AIS data is transmitted in the clear and can be received by anyone with appropriate equipment, or accessed via commercial/free aggregation platforms — making it a widely used OSINT data source, with real limitations.

## How AIS Works

- Vessels broadcast position, speed, heading, and identity at intervals (typically every few seconds to minutes, depending on vessel status)
- Signals are received by coastal base stations and, where coverage allows, satellites
- Aggregator platforms compile this into searchable databases, generally with some processing delay on free tiers
- Broadcast data includes vessel name, flag state, and IMO number; cargo type and destination fields are self-reported by the vessel and not independently verified by the AIS system itself

## Open-Source AIS Platforms Referenced

| Platform | URL | Notes |
|---|---|---|
| MarineTraffic | marinetraffic.com | Widely used free-tier AIS platform; historical data and finer time resolution often require paid access |
| VesselFinder | vesselfinder.com | Offers historical track access, with similar free/paid tiers |
| MyShipTracking | myshiptracking.com | Real-time tracking, free tier |
| Bosphorus Observer | Twitter/X (volunteer-run account) | Manual strait monitoring by individual observers; useful as a supplementary, single-source reference — not a verified institutional feed |

## Intelligence Value of AIS Data

### Pattern-of-Life Analysis
Tracking vessel routines over time can reveal typical traffic patterns; deviations are a useful starting point for further investigation, though they require corroboration before being treated as significant on their own.

### Anomaly Detection
- **AIS spoofing**: vessels transmitting false location data — documented in research by groups such as C4ADS, particularly in sanctions-evasion contexts
- **AIS "going dark"**: vessels turning off transponders, often around sanctioned ports or ship-to-ship transfers
- Unusual port calls or course deviations, when corroborated by other sources

### Sanctions Monitoring
AIS data has been used by researchers and journalists (e.g., CREA, Lloyd's List Intelligence) to track vessels suspected of evading sanctions, including Russian-oil-linked tankers since 2022. These are documented case-by-case findings from named organizations, not outputs of this project's own monitoring.

### Dual-Use Cargo Detection
Cross-referencing AIS-derived movement data with vessel registries and port records can support hypotheses about dual-use or undeclared cargo, but AIS alone cannot confirm cargo contents — manifest data is self-reported and not independently verified.

## Limitations

- AIS transponders can be spoofed or deliberately disabled, and gaps in transmission do not by themselves indicate wrongdoing
- Free platforms have limited historical depth and update frequency compared to paid/institutional feeds
- Cargo and destination fields are self-reported and frequently inaccurate or stale
- Satellite AIS coverage has known gaps, particularly in congested coastal waters and remote areas
- This project does not operate its own AIS receivers or paid data feeds; all findings are drawn from already-published analysis by the cited platforms and organizations

## Application to Turkish Straits

The Turkish Straits are heavily monitored due to their strategic and navigational significance. Official Vessel Traffic Service (VTS) data is supplemented in open-source reporting by volunteer monitoring (e.g., Bosphorus Observer) and commercial AIS platforms — though volunteer, single-observer sources should be treated as indicative rather than verified without independent corroboration.

## Sources

- IMO — AIS Technical Standards (SOLAS Chapter V)
- UNODC — Maritime Crime Programme, AIS-related guidance
- C4ADS — shadow-fleet and AIS-spoofing research methodology
- MarineTraffic — platform/API documentation
- UN Panel of Experts reports referencing sanctions-related maritime monitoring
