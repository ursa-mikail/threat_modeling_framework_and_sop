
| Tool                                      | Primary Focus                    | Type                     | 
| ----------------------------------------- | -------------------------------- | ------------------------ | 
| **[Shodan](https://www.shodan.io)**       | Internet-connected devices       | Network Scanner          |       |
| **[Censys](https://censys.io)**           | Devices, certificates, services  | Network Scanner          | 
| **[Hunter](https://hunter.io)**           | Email address discovery          | OSINT / People Recon     | 
| **[URLScan.io](https://urlscan.io)**      | URL behavior and threat analysis | Threat Analysis          | 
| **[Grep.app](https://grep.app)**          | Source code search               | Code Search              | 
| **[IntelX](https://intelx.io)**           | Breach/darknet/WHOIS search      | OSINT Platform           | 
| **[FullHunt](https://fullhunt.io)**       | Attack surface discovery         | Recon / Security         | 
| **[Vulners](https://vulners.com)**        | Vulnerability database & API     | Threat Intelligence      | 
| **[GreyNoise](https://viz.greynoise.io)** | Scan noise intelligence          | Threat Contextualization | 


# API Attack Types and Mitigations

| **Attack Type**            | **Mitigations**                                                                                   |
|----------------------------|--------------------------------------------------------------------------------------------------|
| Injection                  | Validate and sanitize all data in API requests; limit response data to avoid leaking sensitive data |
| Cross-Site Scripting (XSS) | Validate input; use character escaping and filtering                                              |
| Distributed Denial-of-Service (DDoS) | Use rate limiting and limit payload size                                                    |
| Man-in-the-Middle (MitM)   | Encrypt traffic in transit                                                                        |
| Credential Stuffing        | Use an intelligence feed to identify credential stuffing and implement rate limits               |


# Control Functions and Control Types

| **CONTROL FUNCTIONS** | **CONTROL TYPES** | **Preventative**                                          | **Detective**                                         | **Corrective**                                               |
|-----------------------|-------------------|-----------------------------------------------------------|-------------------------------------------------------|---------------------------------------------------------------|
|                       | **Physical**       | Fences, gates, locks                                      | CCTV and surveillance camera logs                     | Repair physical damage, re-issue access cards                 |
|                       | **Technical**      | Firewall, IPS, MFA solution, antivirus software           | Intrusion detection systems, honeypots                | Patch a system, terminate a process, reboot a system, quarantine a virus |
|                       | **Administrative** | Hiring and termination policies, separation of duties, data classification | Review access rights, audit logs, and unauthorized changes | Implement a business continuity plan or incident response plan |

