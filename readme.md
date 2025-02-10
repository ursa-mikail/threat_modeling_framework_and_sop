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

.... to be continued ...

