# System Security Plan (SSP)
## System Description
The Pseudo Defense System (PDS) is a firewall system that inspects and filter inbound and outbound network traffic at the perimeter of the company's network. The system is used by authorized contractors and company's internal security team to monitor and analyze network activity for potential threats and policy violations. PDS processes metadata and packet-level network traffic coming from external entities accessing services provided by the organization. It does not keep end-user content however, it can log connection details like timestamps, protocol information, and IP addresses for monitoring and auditing purposes. The PDS works within the cloud environment (AWS) and is integrated with upstream and downstream security services like identity management and incident response systems. The system boundary includes cloud-based firewall instances, centralized logging services, and monitoring dashbaords.
## System Categorization
The PDS is categorized as a Moderate impact system based on FIPS 199.
- Confiidentiality: Moderate (network metadata and logs much be protected)
- Integrity: High (log accuracy is critical for incident response)
- Availability: Moderate (system downtime reduces monitoring capability)
  
