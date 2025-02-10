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

#### <u>Notes on Scams and Frauds</u>

##### [Intent]  
###### Scam  
Scams are designed to exploit the victim's gullibility or ignorance. They often rely on the victim's voluntary participation, albeit based on false information.  

###### Fraud  
Fraud involves deliberate deception or misrepresentation with the intention of gaining an unfair or illegal financial advantage.  

##### [Method]  
###### Scam  
Scams often rely on psychological manipulation, persuasion, and the victim's willingness to cooperate. Common types of scams include:  
- Lottery scams  
- Phishing scams  
- Romance scams  

###### Fraud  
Fraud schemes can be more complex and may involve forgery, identity theft, embezzlement, or other forms of financial deception. Types of fraud include:  
- Credit card fraud  
- Insurance fraud  
- Securities fraud  

##### [Victim Involvement]  
###### Scam  
Victims of scams are often active participants, albeit unknowingly. They are convinced to take certain actions, such as:  
- Sharing personal information  
- Sending money  
- Clicking on malicious links  

###### Fraud  
In fraud cases, victims may not be as actively involved. For example, identity theft can occur without the victim's knowledge until they discover unauthorized transactions on their accounts.  

##### [Scale]  
###### Scam  
Scams can target both individuals and organizations but are often smaller in scale, involving fewer victims at a time.  

###### Fraud  
Frauds can be larger in scale and may involve more significant financial losses. Corporate fraud, for instance, can affect a company's financial health and its shareholders.  

##### <b>Countermeasures</b>  
1. **Enable Multi-Factor Authentication (MFA).**  
2. **Enforce the principle of least privilege.**  
3. **Log incidents for legal evidence collection.**  

##### <b>Caveat(s)</b>  
There is also a thin line between offense and defense. Pentesting tools can also be crimeware.  


#### Services

While Endpoints can be seen as infrastructure, they are part of systems. This is the component of interface. Endpoint security involves securing individual devices whether mobile, Internet of Things (IoT), sensors, or any server or client devices that connect to a network. The goal is to prevent malware infections, unauthorized access, and data loss from these device systems. 
Systems also include critical infrastructure systems such as Industrial Control Systems (ICS) like power plants, manufacturing facilities, and utilities from cyber threats that could impact their operations.  
 
This domain provides Intelligence and protects enterprise workloads with threat prevention enabled by machine learning, world-class research, CVE watch and provides automatic remediation for configuration drift. 
Intelligence also includes to ingest log and event data, delivering contextualized visualization of entire infrastructure and security analytics, helping to enhance real-time intrusion detection and policy violation alerts based on user-defined criteria. This is part of comprehensive investigation of security threats, forensics and threat hunting, with network security analytics. 
It provides Multi-tenancy context segregation assurance, Data loss prevention (DLP), log and alert management as well as visualizations of security information across network system to coordinate to improve overall observability. It includes monitoring and responding to storage events, stream data processing, databases changes, code/ executables modifications, Notifications (e.g., SMS, Emails, IoT). 
The domain can be used to identify unused assets, map how security teams work, verify the integrity of a recently deployed system, and identify what technologies are most used. In this way, it can also help organizations save money and identify important opportunities for training. 

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


#### Applications

While platform can be referred to as the <b>architecture, tools and processes</b>, including integrating vendor-specific functions—and often third-party products, that ensure the functions of an entire computing environment, we refer to the computing language platform base that runs within each system. This can be on any layer depending on the language platform (including the different forms of smart contract platforms) in use. 
Domain Specific Language Platform has to be managed and assured differently as they are self-styled by nature. 
Different languages have different `gotchas`, and the version of each language is changing fast. It behooves for the platform specialist to engage a team of specialized experts looking at the idiosyncrasies and flawed implementation that can occur for each language platform. Also note that, language can behave differently on different environments (cloud, mobile, embedded, etc), OS, runtime, hardware, etc. 

#### Protocol, Algorithm and Hardware 
As it may be language Platform related, this will affect the <b>Protocol</b> and <b>Algorithm</b> strata as the users are to be abstracted from the underlying workings and yet be guided by the tool itself on the limitation and scope of safety usage to ensure security being well-implemented and deployed. There has to be caveats if the <b>Hardware</b> and deployment is mobile, distributed, resource and energy limited (e.g. embedded), and/or subjected to hostile or harsh environment, etc. 

<b>Algorithm</b> domain can be on any layer depending on where and how the cryptographic suites are deployed, maintained and designated in usage. 
<b>Protocol</b> piece algorithms to be coordinated into a protocol for safe use and implementation. 
<b>Hardware</b> (+ IoT, embedded) can be on any layer that is designated and deployed for realizing the blockchain operations. 



##### Decompose The Solution (Application, Network, etc) Into Service Segments, Components And Modules 

The examination involves:
**3.1.** Identify Assets and Data Flows 
**3.2.** Subject, Interface and Object (SIO) Analysis 
**3.2.1.** Dependencies 
**3.2.2.** Entry Points and Exit Points 

##### 3.1 Identify Assets and Data Flows

Identify and document the critical assets, data flows, and trust boundaries within the system. Understand how data moves through the system and identify potential points of compromise.  

###### Audit

[1]. Proper documentation must be in-place for clarity on the critical data flow and security boundaries to be delineated. 
This does not include user guide or user set-up guide. Though use cases should be depicted.  
 
Documentations (architecture diagrams describing mechanisms) must be clear and direct to trace the secret generation, flow, and storage. Some fundamental premises must be covered: 
a. Strength of cryptography. 
a.1. What are the cipher suites used, i.e. ciphering, hashing, signing, etc? What are the key lengths used?   
a.2. What are the FIPS certification held by your solution? Is so, please cite them.  
a.3. How do you tend to your data at rest, data-in-transit, and data-in-processing? 
b. What are the secrets in use? What are they used for? (e.g. there should not be the same key for cipher and signing) What are their life-cycles? 
c. The secret generations (i.e. Has the RNG been tested for entropy?). 
d. How are the secrets distributed / populated?  
KMS (key management system) solution: How is your key management system like? i.e. Secrets management lifecycle (from generation to distribution to rotation / revocation to termination, etc). 
e. How did flow and storage ensure that the credentials are well guarded? Is there any point where it is transmitted or stored in plaintext? 
f. How are the secrets (keys, passcodes, etc) protected?   
g. What are the crypto objectives for each of the data objects of interest to be protected? (e.g. video, audio and short text may be ciphered and protected differently. The objective of confidentiality, privacy, integrity, and availability must be set as a clear criteria.) 
h. What are the data / parameters (sensitive/ secret) to be protected? 
- e.g. In some instances, as the SSO (Single-sign on) solutions deployed are using unsigned requests, while the usernames may not be of concern, it is more of how the credentials may be protected in the SSO.  
The known use case(s) must be stated, as certain use cases can affect the security requirements of the implementation. This involves what data and sensitive operations are involved, as well as which zone(s) these operations are running in. 
 
 [2]. Risk / gap analysis 
This includes any risk introduced for the exception to be filed. Which rule is the exception transgressing according to a developed Guide to Cryptography and Deployment Guidelines and/or Cryptographic Controls? State the reasons for the exception or omission. * All the mentioned criteria above are central to arriving at the decision for the exception approval. 
Given the risk / gap analysis, are there any countermeasures introduced to mitigate the risk introduced by the exception? State the effectiveness and limitations or the countermeasures to mitigate the risk introduced by the exception.  
 
a. All applications underwent a formal review process. 
b. Determination and segmentation of certain applications under graded / 1 single trust model. 
c. There is a sufficient detection mechanism to deter traveling private keys and leakage. 
d. The system(s) had undergone a hardening process. 
While filing the exception, always consider the security sufficiency, completeness and correctness aside the functionality to assert for the justification.  
  
[3]. Contingency plans 
State the detection, resistance, and recovery (repair, roll-back and restore) plan. 
 
Assets are documented in the threat model as follows: 
ID: A unique ID is assigned to identify each asset. This will be used to cross-reference the asset with any threats or vulnerabilities that are identified. 
Name: A descriptive name that clearly identifies the asset. 
Description: A description of what the asset is and why it needs to be protected. 
Trust Levels: The level of access required to access the entry point is stated here. These will be referenced with the trust levels with the components the asset is interacting with. 



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

