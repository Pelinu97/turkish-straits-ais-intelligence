# AIS Data Methodology: Open-Source Maritime Intelligence

## Overview

Automatic Identification System (AIS) is a tracking technology mandated by the International Maritime Organization (IMO) for vessels over 300 gross tonnage. AIS data is transmitted publicly and can be monitored by anyone with the right equipment or access to open-source platforms — making it a powerful OSINT tool.

## How AIS Works

- Vessels broadcast their position, speed, heading, and identity every few seconds
- Data is received by coastal stations and satellites
- Aggregated by commercial platforms and made publicly available
- Includes vessel name, flag state, IMO number, cargo type, and destination

## Open-Source AIS Platforms Used

| Platform | URL | Notes |
|---|---|---|
| MarineTraffic | marinetraffic.com | Most comprehensive free AIS platform |
| VesselFinder | vesselfinder.com | Good historical data access |
| MyShipTracking | myshiptracking.com | Real-time tracking |
| Bosphorus Observer | Twitter/X | Manual strait monitoring by volunteers |

## Intelligence Value of AIS Data

### Pattern of Life Analysis
Tracking vessel routines over time reveals normal traffic patterns — deviations from these patterns can indicate significant events.

### Anomaly Detection
- AIS spoofing: vessels transmitting false location data
- AIS silence: vessels deliberately turning off transponders
- Unusual port calls or course deviations

### Sanctions Monitoring
AIS data has been used extensively to track vessels evading sanctions — particularly Russian oil tankers following the 2022 invasion of Ukraine.

### Dual-Use Cargo Detection
Cross-referencing AIS data with vessel registries, cargo manifests, and port records can reveal potential dual-use or illicit cargo movements.

## Limitations

- AIS can be spoofed or disabled
- Free platforms have limited historical data
- Cargo details are often self-reported and unverified
- Satellite AIS coverage has gaps in remote areas

## Application to Turkish Straits

The Turkish Straits are one of the most monitored waterways in the world due to their strategic importance. Volunteer monitoring networks such as the Bosphorus Observer provide real-time open-source intelligence on vessel transits — supplementing official VTS data.

## Sources

- IMO — AIS Technical Standards
- UNODC — Maritime Crime and AIS Monitoring
- C4ADS — Shadow Fleet tracking methodology
- MarineTraffic API Documentation
- UN Panel of Experts — Russia Sanctions Reports
