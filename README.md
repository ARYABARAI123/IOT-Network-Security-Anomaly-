# IoT Network Security Dataset

## Overview

This repository contains a dataset designed for studying IoT network security. Over the span of a week, a series of cyber-attacks were simulated and network traffic was collected, both malicious and benign. The dataset was originally sourced from Kaggle and has been analyzed to provide insights into IoT network behaviors under various conditions.

## Experimentation Overview

### Attacks and Data Collection

- **Monday, October 30th - Recon**
  - Host Discovery: 9:01 - 9:05
  - Ping Sweep: 9:06 - 9:09, 9:12 - 11:04
  - OS Scan: 11:06 - 12:09
  - Vulnerability Scan: 12:10 - 12:16
  - Port Scan: 12:20 - 15:56
  - **Note:** Host Discovery has no representation in extracted features. Fully represented in PCAPs.

- **Tuesday, October 31st - Benign 1**
  - Normal traffic along with various Home Assistant automations: 9:00 - 16:05

- **Wednesday, November 1st - DoS**
  - ICMP Flooding: 9:30 - 9:55
  - Slowloris: 9:58 - 10:26
  - SYN Flood: 10:28 - 10:53
  - UDP Flood: 10:54 - 11:21
  - DNS Flood: 11:23 - 11:49

- **Thursday, November 2nd - Brute Force and Spoofing**
  - Dictionary Brute Force: 9:30 - 11:44
  - ARP Spoofing: 12:12 - 13:48
  - **Note:** ARP Spoofing has limited representation in extracted features. Fully represented in PCAPs.

- **Friday, November 3rd - Benign 2**
  - Normal traffic along with various Home Assistant automations: 9:00 - 16:05

An accompanying timesheet is included with the dataset, providing detailed information about attack and automation timings.

## Dataset Structure

The dataset includes the following files:

- `ACI-IoT-2023.csv`: Labeled dataset containing netflow features.
- `ACI-IoT-2023-Payload.csv`: Labeled dataset using Payload-Byte, an open-source tool for extracting and labeling network packets.
- `pcap_combined/`: A directory containing all PCAP data collected during experimentation.
- `Timesheets/`: A directory containing timestamps for all attacks executed.
- `ACI-IoT-2023-README.docx`: Detailed documentation of the dataset.
- `ACI-IoT-2023-README.txt`: A text version of the dataset documentation.

## Novel Contributions

Our analysis of this dataset provides several new insights:

1. **Dynamic Mix of IoT Devices:**
   - The dataset represents a diverse array of IoT devices, reflecting the heterogeneous nature of contemporary home environments.

2. **Simulated Home Environment:**
   - Provides a realistic simulation of a home IoT network, offering insights beyond traditional lab setups and synthetic environments.

3. **Behavioral Analysis and Holistic Security Evaluation:**
   - Focuses on the behavioral analysis of IoT devices in both normal and adversarial scenarios, allowing for a comprehensive security evaluation.

4. **Multi-Modal Data Representation:**
   - Incorporates multi-modal data, including network traffic patterns, device communication, and device-specific characteristics.

## Data Source
The dataset used for this analysis was sourced from Kaggle.It was adapted and extended through controlled experiments to simulate various cyber-attacks and normal traffic scenarios.
You can access the original dataset [here](https://www.kaggle.com/datasets/emilynack/aci-iot-network-traffic-dataset-2023/data).

