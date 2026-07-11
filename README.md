# Wireshark ICMP Capture

## Overview

This project involves using Wireshark to monitor and analyze ICMP (Internet Control Message Protocol) communication. Individual packet captures were recorded for each target, ensuring that every capture includes exactly **4 ICMP Echo Requests** and **4 ICMP Echo Replies**.


## Files Included

- `google.pcapng` – ICMP capture for **google.com**
- `gateway.pcapng` – ICMP capture for the **10.0.3.15(default gateway)**
- `localhost.pcapng` – ICMP capture for **127.0.0.1 (localhost)**


## Observations

| Target | Result | Observation |
|--------|--------|-------------|
| google.com | ✅ Success | Highest response time due to internet routing. |
| Default Gateway (10.0.3.15) | ✅ Success | Low latency since it is on the local network. |
| 127.0.0.1 (localhost) | ✅ Success | Fastest response because packets never left the local machine. |

## Summary

- **Fastest Target:** 10.0.3.15 (localhost)
- **Slowest Target:** google.com
- **Status:** All packet captures were completed successfully.

