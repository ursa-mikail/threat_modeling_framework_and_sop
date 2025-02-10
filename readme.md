# Threat Modeling Framework and SOP

## Contents
- Introduction  
- Threat Modeling Process  
  - Understand The Context Of The Use Cases Of The Solution  
  - Determine The Strata(s) Involved For The Solution  
  - Decompose The Solution (Application, Network, etc) Into Service Segments, Components And Modules  
  - Determine And Rank Threats  
  - Determine Countermeasures and Mitigation  
  - Address Trade-offs  
- To-do Review Process  

---

## [To-do] section
1. Ease of implementation across more than just our team (this will include presenting, gaining alignment, and training others)  
2. Ability to use a 3rd party tool to facilitate and provide accurate information faster than manual  
3. Ability for us to peer inside of source code, and not get bogged down in the minutia.  
4. Explanations and alignment of how both the tool and framework fit together and work to accelerate each other.  

### To-do Review Process
To ensure the listed tasks are addressed efficiently, the following process will be followed:
- **Task Prioritization:** Rank items based on impact and feasibility.
- **Stakeholder Alignment:** Engage relevant teams for input and agreement.
- **Implementation Plan:** Define milestones, responsible parties, and timelines.
- **Progress Tracking:** Regular status updates and adjustments as needed.

---

## Introduction
This document describes a structured approach to solution threat modeling to identify, quantify, and address the security risks associated with a proposed solution.  
Threat modeling involves examining a system from the perspective of a potential attacker. The threat modeling process comprises the following steps, with documentation recorded at each stage.  

## Threat Modeling Process

### Step 1: Understand the context of the use cases of the solution
The foundational step involves a comprehensive understanding of the context surrounding the use cases of the solution. This initial phase is crucial for establishing a clear framework and identifying the specific scenarios in which the system will operate. By comprehensively grasping the context, threat modeling can be aided with insights into user interactions, data flows, and the overall purpose of the solution.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 1.1 | Ensure alignment on context | Templates, FAQ, requirement documents (e.g. BRS, FRS, SRS) | Stakeholders, Requirements task force (including engineers and architects) | Agreed definitions, assumptions, focus of the problems |
| 1.2 | Identify security principles and goals | Definitions, assumptions, business drivers, policies | Work sessions, surveys, metric collection | Principles and goals |

---

### Step 2: Determine the strata(s) involved for the solution
This step involves identifying the strata(s) involved in the solution, encompassing the 7-strata domain, which includes Infrastructure (Network), Service (including Applications), System, Platform (Computing Language), Protocol, Algorithm, and Hardware.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 2.1 | Develop artifacts to support security requirements | Potential artifacts (e.g., scenarios, misuse/abuse cases, templates) | Work sessions: Identify strata(s) involved | Engineers and architects | Scenarios of misuse/abuse cases, attack models, and scenarios |

---

### Step 3: Decompose the solution (Application, Network, etc) into service segments, components and modules
This step entails breaking down the solution into its service segments, components, and modules for a detailed examination of its structure.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 3.1 | Perform architectural assessments | Architecture diagrams, test logs, and reports | Work sessions: Decompose solution into segments and categorize requirements | Engineers and architects (including security specialists) | Architecture assessment reporting |

---

### Step 4: Determine and Rank Threats
This step involves identifying and prioritizing threats to focus security efforts on the most significant risks.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 4.1 | Perform risk and threat assessments | Security principles and artifacts (misuse/abuse cases, attack models) | Work sessions: Threat modeling frameworks and risk assessments | Engineers and architects (including security specialists) | Risk assessment and threats reporting |

---

### Step 5: Determine Countermeasures and Mitigation
This step involves designing security controls and countermeasures against identified threats.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 5.1 | Determine Countermeasures and Mitigation | Architecture assessment reporting | Work sessions: Countermeasure designs, prototyping/simulation | Engineers and architects (including security specialists) | Countermeasures, Mitigation strategies, Security test exit validation test plans |

---

### Step 6: Address Trade-offs
This step focuses on balancing security measures with system performance and usability.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 6.1 | Address Trade-offs | Countermeasures, Mitigation strategies | Work sessions: Security testing, Performance benchmarking | Engineers and architects (including security specialists) | Security test exit validation tests and reports |

---

## Understand The Context Of The Use Cases Of The Solution
In threat modeling, understanding the context of the solution’s use cases involves an examination of the use case context, often captured in a Business Requirement Specification (BRS). The BRS serves as a foundational document, articulating why the solution exists. It captures environmental nuances and the business landscape in which the solution is expected to operate. The document outlines essential requirements, delineating existing service levels and targeted improvements. It serves as the starting point for proposing preliminary security measures and garnering consensus from stakeholders, ensuring a collective understanding of security objectives before deeper threat analysis.

## Determine The Strata(s) Involved For The Solution
### Define Objectives and Scope
Identify the scope of the threat modeling process, including the network topology, systems architecture, applications, or components to be assessed.

### 7 Strata
A simplified and unified framework can be derived from multiple frameworks, covering 7 strata. The focus is to design countermeasures and defenses against threats across infrastructures, systems, platforms, frameworks, schemes, protocols, and algorithms. The framework ensures observability and controllability of the cybersecurity terrain while overcoming complexity and lack of visibility.

#### The 7-Strata Domains:
1. **Infrastructure — Network**
2. **Service (including Applications)**
3. **System**
4. **Platform (Computing Language)**
5. **Protocol**
6. **Algorithm**
7. **Hardware**

### Infrastructure — Network
This stratum includes network infrastructure (routers, switches, firewalls, etc.) to prevent unauthorized access, network attacks, and data interception. It covers cloud, distributed, and multi-cloud environments, ensuring security against cyber threats. Secure network traffic is crucial across all workloads, whether cloud-based, on-prem, or decentralized.

### Service (including Applications)

The services may include applications, facilities, industrial facilities, banking services, development environment (CI/CD) facilities, or any functions that are manifested into a service. These services may be internal or external, with a business focus, extension, expansion, and continuity. Services can be in the faculty of Governance, Risk, and Compliance (GRC), Identity and Access Management (IAM), Security Operations Center (SOC), Incident Response, Physical Security, etc.

#### Domain of Services

This domain considers defense propositions against threats while providing enterprise-grade application security (Appsec) for web applications and APIs. Enterprises can go beyond traditional rule-based protection and use contextual AI to prevent threats with precision. It includes Posture Management through configuration management services that automate governance processes, visualize and assess security posture, detect insecure configurations, and enforce best practices at scale.

#### Applications

Applications can be porous and fine-grained, comprising 100s of functions, many of which are tiny microservices with their own policies, roles, APIs, and audit trails. This expands the attack surface by adding more entry points with smaller portions of the app behind each one, requiring defense considerations for each entry point.

#### User Protection

This domain covers Application Security Threats to users, including:
1. Account hijacking
2. Credential exposure
3. Oversharing of data
4. DoS attacks
5. Phishing and social engineering
6. Counter scams and frauds
   - Scams: Rely on the victim's voluntary participation and psychological manipulation.
   - Frauds: Involve deliberate deception or misrepresentation to gain financial advantage.
7. Account for human errors by educating users and implementing security tooling.

##### Notes on Scams and Frauds

###### [Intent]
- **Scam:** Designed to exploit the victim's gullibility or ignorance.
- **Fraud:** Involves deliberate deception with the intention of gaining an unfair financial advantage.

###### [Method]
- **Scam:** Often relies on psychological manipulation and victim cooperation.
- **Fraud:** Can involve complex schemes such as forgery, identity theft, and embezzlement.

###### [Victim Involvement]
- **Scam:** Victims actively participate unknowingly.
- **Fraud:** Victims may not be aware until discovering unauthorized actions.

###### [Scale]
- **Scam:** Smaller in scale, involving fewer victims.
- **Fraud:** Larger scale with potentially more significant financial losses.

###### Countermeasures
1. MFA (Multi-factor Authentication).
2. Enforce the principle of least privilege.
3. Log incidents for legal evidence collection.

##### Caveats
- The line between offense and defense is thin; pentesting tools can also be crimeware.

#### System

Endpoints are part of systems and involve securing devices like mobile phones, IoT, sensors, and servers to prevent malware, unauthorized access, and data loss. Critical infrastructure systems like Industrial Control Systems (ICS) must also be protected from cyber threats.

This domain offers Intelligence for enterprise workload protection, including threat prevention enabled by machine learning, CVE watch, and automatic remediation for configuration drift. It also includes real-time intrusion detection and policy violation alerts, network security analytics, and log management.

##### Platform

The platform includes architecture, tools, and processes to ensure the functions of a computing environment. It also involves Domain Specific Language Platforms that require specialized management due to their self-styled nature and the rapid changes in languages and environments.

#### Protocol, Algorithm, and Hardware

Protocols and algorithms ensure security through proper implementation, while hardware (including IoT and embedded systems) is deployed for blockchain operations.

##### Decomposing the Solution

The examination involves:

##### 3.1 Identify Assets and Data Flows

Identify and document critical assets, data flows, and trust boundaries to understand how data moves through the system and identify potential compromise points.

###### Audit

1. Proper documentation must be in place, clearly outlining critical data flow and security boundaries.
2. Documentation (architecture diagrams) must trace secret generation, flow, and storage, including cryptographic strength, secret lifecycle, and key management system (KMS) details.
3. Secrets should be protected throughout their lifecycle.

##### 3.2 Risk/Gaps Analysis

Analyze any risks introduced by exceptions and document countermeasures to mitigate these risks.

##### 3.3 Contingency Plans

State detection, resistance, and recovery plans (repair, rollback, restore).

##### Assets Documentation

Each asset is documented with the following details:
- **ID**: Unique identifier for cross-referencing threats.
- **Name**: Descriptive name of the asset.
- **Description**: Reason for asset protection.
- **Trust Levels**: Access levels required for entry points.


.... to be continued ...

