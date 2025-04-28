# IoT-ZeroTrust-Framework
A Zero Trust-based Intrusion Detection and Prevention System (IDPS) designed for resource-constrained IoT environments, featuring real-time threat analytics, contextual access control, and device-level risk management.

Zero Trust-Based Intrusion Detection and Prevention System (ZT-IDPS) for IoT
📚 Overview
This project presents the design, implementation, and validation of a Zero Trust-based Intrusion Detection and Prevention System (ZT-IDPS) tailored specifically for resource-constrained IoT ecosystems.
The system operationalizes Zero Trust principles—continuous verification, least privilege access, micro-segmentation, and an assumed breach mindset—at the device and network levels.

🚀 Features
Continuous Authentication: Real-time device identity attestation.

Context-Aware Access Control: Dynamic access based on risk profiles.

Lightweight Threat Analytics: Optimized for IoT constraints (limited CPU, memory).

Vulnerability Assessment Module: Firmware, protocol, and service scanning.

Prototype Implementation: Raspberry Pi gateways, ESP32 nodes, and containerized edge computing.

Resilience Testing: Covers attacks like lateral movement, telemetry spoofing, and privilege escalation.

Dataset Integration: Uses TON_IoT, BoT-IoT, and live traffic captures for evaluation.

🛠️ System Architecture
Device Identity Management

Traffic Monitoring and Analysis

Detection Engine (Snort-based with Custom Rules)

Risk Scoring Module

Policy Enforcement and Isolation

Edge Computing Deployment (Dockerized Components)

(You can add an ER diagram or Architecture Diagram here if available.)

🧩 Technologies Used
Programming: Python (backend modules)

IDS Engine: Snort

Web Framework: Flask (for policy management APIs)

Communication Protocols: MQTT, CoAP

Containerization: Docker

Hardware: Raspberry Pi, ESP32 Sensor Nodes

Vulnerability Databases: CVE, CWE

📦 Project Structure
bash
Copy
Edit
zt-idps-iot/
│
├── src/
│   ├── device_manager/          # Device registration, authentication
│   ├── traffic_monitor/          # Real-time packet capture and logging
│   ├── detection_engine/         # Snort rules, anomaly detection scripts
│   ├── policy_enforcer/          # Zero Trust access control
│   ├── risk_assessment/          # Vulnerability scanning and scoring
│
├── datasets/
│   ├── TON_IoT/                  # Public dataset for training/testing
│   ├── BoT_IoT/                  # Public dataset for simulation
│
├── deployment/
│   ├── docker-compose.yml        # Docker deployment file
│   ├── Dockerfile                # Container configuration
│
├── docs/
│   ├── ER_Diagram.png            # ERD of entities and relationships
│   ├── Architecture_Diagram.png  # Overall system architecture
│
├── README.md                     # Project documentation (this file)
├── requirements.txt              # Python dependencies
├── LICENSE
└── .gitignore
🧪 Evaluation
The ZT-IDPS system is evaluated against the following metrics:

Detection Accuracy

Latency

Resource Utilization (CPU, RAM)

Resilience against Advanced Threats

Test Environments:
Public datasets: TON_IoT, BoT-IoT

Simulated IoT traffic on a hybrid testbed with Raspberry Pi and ESP32 nodes.

📈 Results
Mean Time to Detect (MTTD) and Mean Time to Respond (MTTR) were significantly improved compared to traditional IDS solutions.

Low overhead, suitable even for devices with minimal resources.

High detection accuracy in identifying complex threat vectors like lateral movement and privilege escalation.

📜 References
Arun Kumar Bediya, Rajendra Kumar. A Novel Intrusion Detection System for Internet of Things Network Security.

Hyunwoo Lee et al. Intrusion Detection Systems for IoT.

S. Ammer. ZTA-IoT: A Novel Architecture for Zero Trust in IoT Systems.

S. Rose et al. Zero Trust Architecture, NIST SP 800-207.

J. Arshad et al. An Intrusion Detection Framework for Energy Constrained IoT Devices.

M. L. Gambo, A. Almulhem. Zero Trust Architecture: A Systematic Literature Review.

(For full reference list, please see project documentation.)

🤝 Contribution
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

