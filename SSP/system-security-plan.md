# System Security Plan (SSP)
## System Description
The Pseudo Defense System (PDS) is a firewall system that inspects and filters inbound and outbound network traffic at the perimeter of the organization's network. The system is used by authorized contractors and the organization's internal security team to monitor and analyze network activity for potential security threats and policy violations. PDS processes metadata and packet-level network traffic originating from external entities accessing services provided by the organization. It does not store end-user content; however, it logs connection details such as timestamps, protocol information, and IP addresses for monitoring and auditing purposes. The PDS operates within an Amazon Web Services (AWS) cloud environment and is integrated with upstream and downstream security services such as identity and access management (IAM) and incident response systems. The system boundary includes cloud-based firewall instances, centralized logging services, and monitoring dashboards.
## System Categorization
The Pseudo Defense System (PDS) is categorized in accordance with FIPS 199 based on the potential impact to the organization in the event of a security compromise.
- Confidentiality: Moderate (network metadata and logs must be protected)
- Integrity: High (log accuracy is critical for incident response)
- Availability: Moderate (system downtime reduces monitoring capability)
  
Based on these impact levels, the overall system categorization for PDS is HIGH.

## System Control Selection

The Pseudo Defense System (PDS) security controls are selected in accordance with NIST SP 800-53 based on the system's HIGH-impact categorization

The HIGH baseline controls are applied to ensure adequate protection of system confidentiality, integrity, and availability. The following controls have been identified as key security controls for the PDS:

**AC-2 (Account Management)
Ensures that users account for contractors and internal personnel are properly managed, including account creation, modification, and removal. 

**IA-2 (Identification and Authentication)
Requires users to authenticate using secure mechanisms before accessing the system.

**AU-2 (Audit Events)
Defines the types of events that must be logged, including network traffic and access activity.

**AU-6 (Audit Review, Analysis, and Reporting)
Ensures that logged events are regularly reviewed and analyzed for suspicious activity.

**SI-4 (System Monitoring)
Provides continuous monitoring of network traffic to detect potential threats and anomalies.

**SC-7 (Boundary Protection)
Enforces network traffic filtering at the system boundary through firewall rules and inspection mechanisms.

These controls support the system's ability to detect, prevent, and respond to security incidents within the cloud environment.
