# Methodology

This document tracks the step-by-step workflow used for authorized internal network discovery and service enumeration. IP addresses have been redacted for security hygiene.
## Step 1: Scope Definition and Network Baseline

Before performing any scanning activity, I defined the authorized scope of the assessment.

Using local system networking commands, I identified my host system’s IPv4 address and the default gateway. This confirmed that the assessment would be limited to a private IPv4 LAN in the 192.xxx.x.x/xx subnet.

The default gateway (192.xxx.x.x) was identified as the primary network infrastructure device. All subsequent scanning activity was restricted to this authorized network range.

## Step 2: Host Discovery

Host discovery was conducted on an authorized private IPv4 /24 subnet to establish a baseline inventory of active network assets.

Using Nmap in discovery-only mode, the scan identified live hosts without performing port or service enumeration. This approach minimized network impact while providing visibility into which IP addresses were actively responding on the network.

At this stage, only asset existence was documented. Device type, vendor information, services, and security posture were intentionally deferred to later steps to follow a structured, incremental analysis workflow.

Redacted scan evidence for this step is stored in `evidence/01_host_discovery_redacted.txt`, and identified hosts were recorded in the asset inventory table for subsequent enrichment.
