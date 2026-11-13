# Zenmap Network Discovery Lab

This project documents a Zenmap Quick Scan on a local Wi-Fi subnet and shows how to verify which hosts were up and visualize their topology.

## Lab Overview

| Component | Configuration |
|---|---|
| Platform | Windows |
| Tool | Zenmap, the Nmap graphical interface |
| Scan profile | Quick Scan |
| Scope | Local Wi-Fi subnet with a /24 prefix |

## Objectives

- Use Windows IP configuration to identify the local IPv4 address and subnet mask.
- Review the Quick Scan output for live hosts.
- Match the scan results to the topology view and save a PDF.

## Result Validation

Zenmap reported **3 hosts up** in the selected scan. These were the default gateway, the Windows computer running Zenmap, and one other device. Zenmap showed MAC addresses for the two remote devices. Windows IP configuration provided the local computer’s MAC address.

The topology view contained an additional address from a different subnet. The selected scan’s summary gave the count for this lab.

## What I Learned

The subnet mask determines the target range. When Zenmap displays results from multiple scans, the summary for the selected scan is the best place to confirm the host count for that target.

## Evidence

| View | Observation |
|---|---|
| Nmap Output | 256 addresses checked, 3 hosts up |
| Topology | The view displayed the three scan results and one address from another subnet |

## Skills Demonstrated

- Reading IPv4 configuration and CIDR notation
- Interpreting Zenmap host discovery results
- Documenting network topology with identifying details redacted

## Course Credit

Thanks to NetworkWalks and Waqas Karim CCIE for the lab guidance.
