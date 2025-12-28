# Methodology

This document tracks the step-by-step workflow used for authorized internal network discovery and service enumeration. IP addresses have been redacted for security hygiene.
## Step 1: Scope Definition and Network Baseline

Before performing any scanning activity, I defined the authorized scope of the assessment.

Using local system networking commands, I identified my host system’s IPv4 address and the default gateway. This confirmed that the assessment would be limited to a private IPv4 LAN in the 192.xxx.x.x/xx subnet.

The default gateway (192.xxx.x.x) was identified as the primary network infrastructure device. All subsequent scanning activity was restricted to this authorized network range.
