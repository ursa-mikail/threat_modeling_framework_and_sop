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

##### To-do Review Process
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

**Step 1**: Understand the context of the use cases of the solution  
**Step 2**: Determine the strata(s) involved of the solution  
**Step 3**: Decompose the solution (Application, Network, etc) into service segments, components and modules  
**Step 4**: Determine and Rank Threats  
**Step 5**: Determine Countermeasures and Mitigation  
**Step 6**: Address Trade-offs  


### Step 1: Understand the context of the use cases of the solution
The foundational Step 1 involves a comprehensive understanding of the context surrounding the use cases of the solution. This initial phase is crucial for establishing a clear framework and identifying the specific scenarios in which the system will operate. By comprehensively grasping the context, threat modeling can be aided with the insights of the intricacies of user interactions, data flows, and the overall purpose of the solution. This contextual awareness lays the groundwork for the subsequent steps in the threat modeling process, enabling a more precise and targeted analysis of potential security threats. Effectively discerning the use cases ensures that the threat modeling exercise aligns closely with the actual operational environment, enhancing the relevance and accuracy of the security assessments conducted in later stages.  

#### Step Breakdown
|   | Step | Input | Means | Participants | Output |
|------|------|-------|-------|-------------|--------|
| 1.1 | Ensure that everyone aligns on the same context, i.e. agree on definitions, assumptions, focus of the problems. etc. | Templates of definitions, FAQ, requirement documents (e.g. BRS, FRS, SRS), etc. | 1. Set up focus group 2. Structured interviews 3. Create FAQ| Stakeholders, Requirements task force (including engineers and architects) | Agreed definitions, assumptions, focus of the problems |
| 1.2 | Identify security principles and goals | Definitions, assumptions, focus of the problems, candidate goals, business drivers, policies and procedures, example | Conduct work sessions, surveys, collect metrics, etc. | Stakeholders, Requirements task force (including engineers and architects) | Principles and goals |

---

### Step 2: Determine the strata(s) involved for the solution
Step 2 of the threat modeling process involves identifying the strata(s) involved of the solution, encompassing the 7-strata domain, which includes Infrastructure (Network), Service (including Applications), System, Platform (Computing Language), Protocol, Algorithm, and Hardware.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 2.1 | Develop artifacts to support security requirements | Potential artifacts (e.g., scenarios, misuse/abuse cases, templates) | Work sessions: Identify strata(s) involved | Engineers and architects | Scenarios of misuse/abuse cases, attack models, and scenarios |

---

### Step 3: Decompose the solution (Application, Network, etc) into service segments, components and modules
Step 3 entails the decomposition of the solution, which may comprise the application, network, and other elements, into service segments, components, and modules. This deconstruction allows for a detailed examination of the various building blocks within the system, providing a comprehensive understanding of its structure. 
 

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 3.1 | Perform architectural assessments | Architecture diagrams, test logs, and reports | Work sessions: Decompose solution into segments and categorize requirements | Engineers and architects (including security specialists) | Architecture assessment reporting |

---

### Step 4: Determine and Rank Threats
Step 4 involves determining and ranking threats. This critical phase requires a meticulous analysis of potential vulnerabilities and risks associated with each identified component or module. By prioritizing these threats, security teams can focus their efforts on addressing the most significant and impactful risks to the system.   

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 4.1 | Perform risk and threat assessments | Security principles and artifacts (misuse/abuse cases, attack models) | Work sessions: Threat modeling frameworks and risk assessments | Engineers and architects (including security specialists) | Risk assessment and threats reporting |

---

### Step 5: Determine Countermeasures and Mitigation
Step 5 is in determining countermeasures and mitigation strategies. This involves devising proactive measures and security controls to safeguard against the identified threats. Countermeasures may include implementing encryption protocols, access controls, or other security mechanisms tailored to address specific vulnerabilities within the system.  

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 5.1 | Determine Countermeasures and Mitigation | Architecture assessment reporting | Work sessions: Countermeasure designs, prototyping/simulation | Engineers and architects (including security specialists) | Countermeasures, Mitigation strategies, Security test exit validation test plans |

---

### Step 6: Address Trade-offs
Step 6 addresses trade-offs. This stage acknowledges that implementing security measures can sometimes introduce trade-offs, such as performance impacts or usability constraints. Security professionals must carefully weigh these trade-offs and make informed decisions to strike a balance between robust security and maintaining the system's functionality and user experience. 

#### Step Breakdown
| Step | Input | Means | Participants | Output |
|------|-------|-------|-------------|--------|
| 6.1 | Address Trade-offs | Countermeasures, Mitigation strategies | Work sessions: Security testing, Performance benchmarking | Engineers and architects (including security specialists) | Security test exit validation tests and reports |

---

## Understand The Context Of The Use Cases Of The Solution
In threat modeling, the equivalent of understanding the context of the solution's use cases involves examination of use case context. This can be captured in a document such as the Business Requirement Specification (BRS). The BRS serves as a foundational document, encapsulating the entirety of requirements articulating why the solution exists. This document is instrumental in capturing the environmental nuances and business landscape within which the solution is expected to operate. It outlines the essential requirements that the system must fulfill, delineating the existing service level and the targeted improvements it aims to achieve. It serves as the starting point to propose preliminary security measures and garner consensus from stakeholders, ensuring a collective understanding of the security objectives. This sets the stage for a more in-depth exploration of potential threats in subsequent phases of the threat modeling process. 

## Determine The Strata(s) Involved For The Solution
### Define Objectives and Scope
Identify the scope of the threat modeling process, including the network topology, systems architecture, applications, or components to be assessed. 

### 7 Strata
A simplified and unified framework can be derived from multiple frameworks. The framework covers 7 strata. The focus is to have countermeasures and defenses designed against threats for the domains of infrastructures, systems, platform frameworks, schemes, protocols, and algorithms. 

The 7-strata domain framework is derived as a common denominator that covers the frameworks mentioned above. The idea is to capture the observability and controllability of the cybersecurity terrain addressed. The crux is to overcome complexity and the lack of visibility. 


#### The 7-Strata Domains:
1. **Infrastructure — Network**
2. **Service (including Applications)**
3. **System**
4. **Platform (Computing Language)**
5. **Protocol**
6. **Algorithm**
7. **Hardware**

### Infrastructure — Network
This stratum includes Network (network infrastructure, including routers, switches, firewalls, and other network devices). It involves measures to prevent unauthorized access, network attacks, and data interception, i.e. ingress and outgress of the network security boundary (perimeter). The network can be in the form of Cloud or other distributing computing topologies.  
 
This domain covers how the nodes are connected, and how they can be disconnected, which can pose MitM denial or attacks, e.g. network partitioning or division. Many enterprise environments are multi-cloud and multi-network connectivity. The complexity of configuration management, granular monitoring across platforms, and access control often lead to disjointed workflows that involve manual configuration and limit visibility exacerbates security challenges. 
This threat modeling on this domain covers how to secure network traffic wherever workloads run whether Cloud, on-prem or decentralized or distributed networks. Workload Protection protects system and network workloads end-to-end from source code to production. Gives enterprises (cloud, network, etc) agnostic unified visibility and threat prevention across apps, APIs, K8s clusters, and serverless functions. 
 
It is important to know where the domain boundaries are, and how each domain works seamlessly in tandem with each other. Firewalls protect services from the Internet. Malware shields within. The perimeter network security must be sufficient against cyber threats, even when data or workloads sit in the cloud. 

### Service (including Applications)

The services may be application, facilities, industrial facilities, banking services, development environment (CI/CD) facilities, etc, or any faculties that are represented, presented and manifest itself into a service. Services may be internal. This can be in the faculty of Governance, Risk, and Compliance (GRC, aligning security practices with its business objectives, assessing and managing risks, and ensuring compliance with industry regulations and standards), Identity and Access Management (IAM) as a form of Control, Security Operations Center (SOC, centralized team responsible for monitoring, detecting, analyzing, and responding to security incidents in real-time) as a form of Command and Control, Incident Response (Restoration and Recovery, Reformation and Refinement), Physical Security (securing physical assets, facilities, and equipment to prevent unauthorized access, theft, and other physical threats), etc. 
Services may be external for business focus, extension, expansion and continuity.  
 
This domain of services considers the defense propositions (against threats) when providing enterprise-grade application security (Appsec) for web applications and APIs. Enterprises can go beyond traditional rule-based protection and leverage the power of contextual AI to prevent threats with a high level of precision. 
It subsumes Posture Management by configuring governing policies via configuration management service systems. It automates the process of governance and enables enterprises to visualize and assess overall enterprise security posture, detect insecure configurations, and enforce best practices at scale. 
 
Applications can be porous and fine-grained. Comprising 100s of functions, many applications are tiny microservices with its own policies, role, API, audit trail, etc. This changes the attack surface, instead of a small number of entry points with lots of functionality hidden behind each one, there are now more entry points, each with a small part of the app behind it. Defending the application now requires thinking about each entry point. 
 
The domain covers user protection such as Application Security Threats to users. This includes: 
1. Account hijacking 
2. Credential exposure: Exposing credentials can lead to account hijacking and a wide range of sophisticated long-term attacks. 
3. Oversharing of data 
4. DoS attacks 
5. Phishing and social engineering 
6. Counter scams and frauds 
* Scams tend to rely on the victim's voluntary participation and psychological manipulation, while frauds involve more deliberate, often complex acts of deception and can lead to more serious legal consequences. 
7. Account for the human aspect: User error is one of the most common causes of data breaches. Taking a 2-pronged approach of user education and implementing security tooling such as URL filters, anti-malware, and intelligent firewalls can reduce the risk of social engineering leading to a catastrophic security issue. 


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


1. **Trust Levels**

| ID     | Name                      | Description                                                                                                                                                                                                                                                                                                   |
|--------|---------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CD_001 | Customer Database          | The database contains personally identifiable information (PII) of registered users, including names, addresses, and contact details. It is an asset for customer interactions and must be protected to ensure privacy and compliance with data protection regulations.                               |
| PG_001 | Payment Gateway            | The gateway facilitates secure online transactions, processing credit card information and financial data. This component is pivotal for the revenue stream of the application and demands protection to prevent unauthorized access or tampering.                                                             |
| SM_001 | Session Monitor            | The agent component is critical for tracking and managing user sessions within the application. It plays a crucial role in maintaining user authentication and authorization states, ensuring a secure and seamless user experience. The Session Monitor stores session tokens, user privileges, and other session-related data. |
|        | **Trust Levels Documentation** | Trust levels are documented in the threat model as follows:                                                                                                                                                                                                                                                                      |

2. **Trust Levels Description**

| ID        | Name                            | Description                                                                                                                                                                                              |
|-----------|---------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| AS_001    | Authorized application servers  | Servers that serve as an intermediary between the client and the database.                                                                                                                                                                                                 |
| MS_001    | Microservices                   | Microservices may have their own databases or share a common database. Each microservice is responsible for managing its data and may interact with the database independently.                                                |
| PPM_001   | Payment processing module       | A dedicated payment processing module or service within the system is designed to interact specifically with the payment gateway. This module handles the creation of payment requests, processing responses from the payment gateway, and managing the overall payment flow. |
| BES_001   | Back-end server or middleware   | A back-end server or middleware may play a role in orchestrating communication between different components of the system and the payment gateway. It ensures that the necessary data is transmitted securely and that responses from the payment gateway are appropriately handled.       |
| SMW_001   | Security middleware             | Security middleware components, including intrusion detection systems or web application firewalls, may access the Session Monitor to monitor and analyze session-related activities for potential security threats or anomalies.                                |
| LAS_001   | Logging and auditing systems    | Logging and auditing systems may integrate with the Session Monitor to record session-related events and activities. This integration supports security auditing, compliance, and forensic analysis.                                            |

3. **Subject, Interface, and Object (SIO) Analysis**

- **Purpose**: Architecture draws the engineering paradigm to work out the components, relationships (and interactions/interface) of the functioning ecosystem to fulfill or manifest an enabling phenomenon. Architecture also helps us to understand the system. It is a blueprint to tool and capture the comprehension for both analysis and synthesis of solutions.
- **Dependencies and Risk**: Recognizing that a system can only be as secure as its weakest link. Problems with inconsistent naming, poorly-defined boundaries, highly-coupled interfaces and systems, and ambiguity in definitions or consideration of any condition are hints to a future disaster.
- **Subjects, Interfaces, and Objects**: Each entity must be carefully profiled and registered, ensuring trustworthiness before engaging in secure transactions.

**4. Diagrams for Architectural Representation**

1. **User Case**: A high-level view of the system from a user's perspective, showcasing interactions between users and the system.
2. **Timing, Swimlane (Sequence)**: Illustrates the chronological order of interactions between different components or actors in the system over time.
3. **Flow Chart**: A step-by-step representation of processes and decision-making within the system.
4. **State Machine**: Represents the different states that a system or component can exist in and the transitions between these states in response to events.
5. **Block-Component Flow**: Depicts the major components of the system as blocks or modules and illustrates the flow of data or control between them.
6. **Entity-Relationship**: Models the relationships between different entities (such as database tables) within the system.

**5. Dependencies Documentation**

| ID     | Description                                                                                                                                       |
|--------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| LIB001 | Third-party library for cryptographic functions. This dependency is utilized to enhance the application's security by implementing robust encryption algorithms. |
| FW002  | Represents the firewall solution integrated into the application's infrastructure, providing a crucial layer of defense.                          |
| API003 | External API for Payment Processing. This dependency facilitates communication with a third-party payment processing service.                      |

**6. SDLC and SBoM**

The defensive SDLC emphasizes traceable details for forensics. SBoM formats are encouraged for dependency management and software lifecycle management.
"""



.... to be continued ...

