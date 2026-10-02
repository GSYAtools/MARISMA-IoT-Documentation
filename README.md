# MARISMA-IoT Research Artifacts

This repository contains a compact set of research artifacts supporting **MARISMA-IoT**, a risk-analysis and risk-management pattern for heterogeneous Internet of Things (IoT) environments. The material is organized into three complementary PDF documents covering the core taxonomies of the pattern, the relationships among its main elements, and the asset inventory used in the laboratory Smart Home case study.

## Repository contents

| Document | Purpose |
|---|---|
| [`Basic_Artifacts_MARISMA-IoT_Pattern.pdf`](./Basic_Artifacts_MARISMA-IoT_Pattern.pdf) | Defines the main reusable artifacts of the MARISMA-IoT pattern: asset families and types, threat families and types, security domains, and impact dimensions. |
| [`Relationship_Matrices_MARISMA-IoT_Pattern_unified.pdf`](./Relationship_Matrices_MARISMA-IoT_Pattern_unified.pdf) | Provides the relationship matrices connecting domains, security objectives, threat families, asset families, threat types, and affected dimensions. |
| [`Assets_MARISMA-IoT_Case_Study_Laboratory_Smart_Home.pdf`](./Assets_MARISMA-IoT_Case_Study_Laboratory_Smart_Home.pdf) | Instantiates the asset taxonomy in the laboratory Smart Home used as the MARISMA-IoT case study. |

---

## 1. Basic artifacts of the MARISMA-IoT pattern

The basic-artifacts document consolidates the reusable knowledge required to instantiate MARISMA-IoT in an IoT environment.

### 1.1 Asset taxonomy

The pattern defines **25 asset types grouped into 9 asset families**.

| Asset family | Asset types |
|---|---|
| **IoT Devices** | Hardware; Software; Sensors; Actuators; Sensors/Actuators |
| **Other IoT Ecosystem Devices** | Devices to interface with Things; Devices to manage Things; Embedded systems |
| **Communications** | Networks; Protocols |
| **Infrastructure** | Routers; Gateways; Power supply; Security assets |
| **Platform & Backend** | Web-based services; Cloud infrastructure and services |
| **Decision Making** | Data mining; Data processing and computing |
| **Applications & Services** | Data analytics and visualisation; Device and network management; Device usage |
| **Information** | At rest; In transit; In use |
| **Audio/Visual** | Digital Streaming Output Systems |

This taxonomy covers physical devices, software, communication mechanisms, infrastructure, cloud and backend services, information assets, management functions, analytics, and multimedia components.

### 1.2 Threat taxonomy

The consolidated threat catalog contains **75 threat types grouped into 15 threat families**.

| Threat family | Number of threat types | Examples |
|---|---:|---|
| **Nefarious activity / Abuse** | 7 | Malware, exploit kits, targeted attacks, DDoS, malicious devices, privacy attacks, information modification |
| **Eavesdropping / Interception / Hijacking** | 5 | Man-in-the-middle/replay, protocol hijacking, information interception, reconnaissance, session hijacking |
| **Outages** | 3 | Network outage, device/system failure, loss of support services |
| **Damage / Loss (IT Assets)** | 1 | Sensitive-information leakage/disclosure |
| **Failures / Malfunctions** | 2 | Software vulnerabilities, third-party failures |
| **Disaster** | 2 | Natural disaster, environmental disaster |
| **Physical attacks** | 2 | Device modification, device/media destruction or sabotage |
| **Legal** | 4 | Breach of legislation, court order, domain seizure, contractual non-compliance |
| **Physical threats** | 6 | Fire, water, harmful radiation, major accident, explosion, dust/corrosion/freezing |
| **Natural threats** | 6 | Climatic, seismic, volcanic and meteorological phenomena, flood, pandemic/epidemic |
| **Infrastructure failures** | 7 | Supply-system failure, cooling/ventilation failure, power loss, telecommunications failure, electromagnetic/thermal effects |
| **Technical failures** | 2 | Information-system saturation, maintainability violation |
| **Human actions** | 21 | Social engineering, spying, credential theft, unauthorized use, malware distribution, data corruption, physical intrusion, etc. |
| **Compromise of functions or services** | 4 | Error in use, abuse/forging of permissions, denial of actions |
| **Organizational threats** | 3 | Lack of staff, lack of resources, failure of service providers |

Threat codes preserve the identifiers available in the source taxonomies, including prefixes such as `TP`, `TN`, `TI`, `TT`, `TH`, `TC`, and `TO`. Threats that did not originally provide an explicit identifier are assigned a MARISMA-IoT code using the `MI-` prefix.

### 1.3 Security domains

The consolidated domain catalog combines IoT-oriented cybersecurity management areas with ISO/IEC-aligned control domains.

#### IoT-oriented domains

- Asset Management
- Identity and Access Management (IAM)
- Configuration and Change Management
- Data Protection
- Vulnerability Management
- Incident Detection and Response
- Information Security Awareness, Education and Training

#### ISO/IEC-aligned domains

- Organizational
- People
- Infrastructure
- Technology

Together, these domains structure the security objectives and controls used to manage organizational, human, physical/infrastructure, and technological risk across the IoT lifecycle.

### 1.4 Impact dimensions

MARISMA-IoT evaluates the consequences of threats through **8 dimensions**:

| Dimension | Scope |
|---|---|
| **Privacy** | Protection of personal, sensitive, behavioral, and usage information. |
| **Safety** | Potential physical harm to occupants or users caused by compromised IoT functions. |
| **Reliability** | Correct and dependable operation of devices, services, sensors, actuators, and control components. |
| **Resilience** | Ability to withstand, adapt to, and recover from attacks, failures, or adverse conditions. |
| **Integrity** | Physical integrity of devices and logical integrity of data, commands, and system state. |
| **Availability** | Continued accessibility and operation of devices, services, and critical functions. |
| **Legality** | Compliance with applicable laws, regulations, contractual obligations, and legal requirements. |
| **Accountability** | Responsibility, auditability, traceability, transparency, and evidence of security actions. |

---

## 2. Relationship matrices of the MARISMA-IoT pattern

The relationship-matrices document operationalizes the pattern by linking its main reusable artifacts.

### 2.1 Domain–Objective–Threat Family Matrix

The first matrix connects:

**Security Domain → Security Objective / Control → Threat Family**

It contains **93 security objectives/controls**, organized into four main domains:

- Organizational
- People
- Physical
- Technological

Each objective is mapped to the threat families that it contributes to mitigating. The matrix covers eight high-level threat families:

1. Nefarious activity / Abuse
2. Eavesdropping / Interception / Hijacking
3. Outages
4. Damage / Loss (IT Assets)
5. Failures / Malfunctions
6. Disaster
7. Physical attacks
8. Legal

This matrix provides traceability between the control structure of the pattern and the risk scenarios that each objective is intended to address.

### 2.2 Asset–Threat–Dimensions Matrix

The second matrix connects:

**Threat Family → Threat Type → Asset Family → Affected Dimensions**

It includes **29 representative threat types** and the following **9 asset families**:

- IoT Devices
- Other IoT Ecosystem Devices
- Communications
- Infrastructure
- Platform & Backend
- Decision Making
- Applications & Services
- Information
- Audio/Visual

For each relevant threat–asset relationship, the matrix identifies the impact dimensions that may be degraded.

#### Dimension abbreviations used in the matrix

| Code | Dimension |
|---|---|
| `P` | Privacy |
| `S` | Safety |
| `C` | Reliability |
| `RL` | Resilience |
| `I` | Integrity |
| `D` | Availability |
| `L` | Legality |
| `RP` | Accountability |

The matrix is intended to support structured risk calculation, control prioritization, and consistent reuse of knowledge across IoT scenarios.

---

## 3. MARISMA-IoT laboratory Smart Home case study

The case-study PDF instantiates the MARISMA-IoT asset taxonomy in a **physical Smart Home testbed deployed in a laboratory**.

The testbed combines heterogeneous devices and services using technologies such as Wi-Fi, ZigBee, MQTT, HTTP/HTTPS, local automation, edge processing, and proprietary cloud platforms.

### 3.1 Case-study asset inventory

The inventory contains **32 concrete or logical assets** distributed across the MARISMA-IoT asset families.

| Asset family | Asset type | Case-study asset | Model / implementation |
|---|---|---|---|
| IoT Devices | Hardware | Embedded microcontroller of the IoT devices | Generic |
| IoT Devices | Software | Internal firmware of the IoT devices | Generic |
| IoT Devices | Sensors | Temperature and humidity sensor | Generic |
| IoT Devices | Sensors | Motion sensor | Tuya ZigBee Motion Sensor ZMIR01 |
| IoT Devices | Actuators | Smart bulb | Moes E27 |
| IoT Devices | Actuators | Automated blind motor | Generic |
| IoT Devices | Actuators | Smart switch | MOES ZigBee Smart Switch ZS-EUB & MOES WiFi Smart Switch ZS-EUB |
| IoT Devices | S/A (Sensor/Actuator) | Smart thermostat | MOES BHT-006GAW Series WiFi Thermostat |
| IoT Devices | S/A (Sensor/Actuator) | Smart plug | ZigBee Power Plug-001SPB2 & Athom Smart Plug PG01 |
| IoT Ecosystem | Interface Devices | Smart display with voice assistant | Google Nest Hub 2 & Amazon Echo Show 5 |
| IoT Ecosystem | Management Devices | Smart home hub | Raspberry Pi 4 + ConBee II + Home Assistant |
| IoT Ecosystem | Embedded Systems | Raspberry Pi mini-computer | Raspberry Pi 4 |
| Communications | Networks | Home Wi-Fi network and ZigBee network | Generic |
| Communications | Protocols | Wi-Fi protocol | Generic |
| Communications | Protocols | MQTT protocol | Generic |
| Communications | Protocols | ZigBee protocol | Generic |
| Communications | Protocols | HTTP/HTTPS protocol | Generic |
| Infrastructure | Routers | Home Wi-Fi router | TP-Link Archer MR200 |
| Infrastructure | Gateways | Multi-protocol gateway | SONOFF B09ZQQZSQZ |
| Infrastructure | Power Sources | Rechargeable lithium battery in compatible IoT devices | Generic |
| Infrastructure | Security Assets | WPA2 encryption on Wi-Fi network and secure credentials | Generic |
| Platform and Backend | Web Services | Open-source home automation software platform | Home Assistant |
| Platform and Backend | Cloud Infrastructure and Services | Cloud-based AIoT platform | Tuya AIoT Cloud & AWS IoT Cloud Platform |
| Decision Making | Data Mining | Artificial intelligence algorithm in the cloud | Generic |
| Decision Making | Processing and Computing | Edge computing | Generic |
| Applications and Services | Data Analysis and Visualization | Grafana dashboard for IoT | Generic |
| Applications and Services | Device and Network Management | Unified home automation control app | Home Assistant |
| Applications and Services | Device Usage | Context-based automation | Generic |
| Information | At Rest | Stored historical data | Generic |
| Information | In Transit | IoT message in transmission | Generic |
| Information | In Use | Data used in real time | Generic |
| Audio/Visual | Digital Streaming Systems | Smart TV | Chromecast 3 |

### 3.2 Architecture represented by the inventory

The asset inventory represents a heterogeneous Smart Home architecture including:

- **Wi-Fi IoT devices** connected through a domestic wireless router.
- **ZigBee sensors and actuators** integrated through a coordinator.
- A **Raspberry Pi 4** acting as a local integration and automation node.
- **Home Assistant** for device management, automation, monitoring, and visualization.
- **MQTT-based communications** for lightweight publish/subscribe interaction.
- **HTTP/HTTPS communications** for local and remote service interaction.
- **Cloud dependencies**, including Tuya AIoT Cloud and AWS IoT Cloud Platform.
- **Voice-assistant and multimedia devices**, including Google Nest Hub, Amazon Echo Show, and Chromecast.
- **Security-related assets**, including WPA2 protection and access credentials.
- **Information in different states**: at rest, in transit, and in use.

This testbed provides a controlled environment in which MARISMA-IoT can instantiate its asset taxonomy and apply the relationships among assets, threats, dimensions, controls, and security objectives.

---

## 4. How the three PDFs fit together

The documents should be read as three layers of the same MARISMA-IoT knowledge model:

```text
Basic Artifacts
      │
      ├── Asset taxonomy
      ├── Threat taxonomy
      ├── Security domains
      └── Impact dimensions
      │
      ▼
Relationship Matrices
      │
      ├── Domain ─ Objective ─ Threat Family
      └── Threat ─ Asset Family ─ Dimension
      │
      ▼
Laboratory Smart Home Case Study
      │
      └── Concrete assets instantiated from the reusable taxonomy
```

In practical terms:

1. **The basic artifacts define what can be modeled.**
2. **The relationship matrices define how the elements are connected.**
3. **The Smart Home case study shows how the reusable model is instantiated in a concrete IoT environment.**

---

## 5. Intended use

These artifacts can be used to support:

- IoT asset identification and classification.
- Threat identification and structured threat modeling.
- Multidimensional impact assessment.
- Traceability between security objectives and threat families.
- Identification of relevant threat–asset relationships.
- Security-control prioritization.
- Reuse of risk knowledge across heterogeneous IoT environments.
- Instantiation of MARISMA-IoT in eMARISMA or equivalent risk-analysis workflows.

---

## 6. Source manuscript

The artifacts summarized in this repository are derived from the MARISMA-IoT research work:

> **MARISMA-IoT: A Standards-Aligned Risk Management Framework for Smart IoT Systems**

The associated case study evaluates the practical application of the pattern through a laboratory Smart Home containing heterogeneous IoT devices, protocols, local control components, and cloud dependencies.

---

## 7. Scope note

The Smart Home is a **laboratory case study** used to instantiate and evaluate the MARISMA-IoT pattern. The reusable taxonomies and matrices are intended to represent a broader IoT risk-management knowledge base and are not limited to domestic IoT environments.
