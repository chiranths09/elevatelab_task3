Basic Vulnerability Assessment Using OpenVAS (GVM)
Objective

The objective of this project is to perform a vulnerability assessment on a system using a standard security tool and identify potential security weaknesses. This task helps in understanding how vulnerabilities are detected, analyzed, and mitigated in real-world environments.

Tool Used
OpenVAS (Greenbone Vulnerability Management - GVM)
System Details
Operating System: Kali Linux
Target: Localhost (127.0.0.1)
Scan Type: Full and Fast
Scan Duration: 30–60 minutes
Methodology
Installed and configured OpenVAS (GVM)
Updated vulnerability feeds and initialized the database
Accessed the web interface via a browser
Created a target using localhost (127.0.0.1)
Configured a scan task using the “Full and Fast” profile
Executed the vulnerability scan
Analyzed the scan results
Documented identified vulnerabilities and mitigation steps
Scan Summary
Total Vulnerabilities Detected: 19
Informational: 18
Medium Severity: 1
High Severity: 0
Critical Severity: 0
Identified Vulnerability
Vulnerability Name: SSL/TLS Medium Strength Cipher Suites Supported
Severity Level: Medium
CVSS Score: 5.9
Description

The scan identified that the system supports SSL/TLS cipher suites classified as medium strength. These cipher suites may not provide strong encryption and could allow attackers to compromise secure communication.

Technical Explanation

SSL/TLS protocols are used to secure communication over networks. Cipher suites define how encryption is performed. Medium-strength cipher suites use weaker encryption algorithms compared to modern standards, making them less secure.

Impact
Possible interception of encrypted communication
Increased risk of Man-in-the-Middle attacks
Potential exposure of sensitive data
Affected Component
SSL/TLS configuration of local services
Recommended Mitigation
Disable medium-strength cipher suites
Enable strong encryption algorithms such as AES
Use TLS 1.2 or TLS 1.3
Regularly update SSL/TLS configurations
Apply the latest system and security updates
Informational Findings
Operating system identification
Service detection
SSL certificate details
Hostname reporting
CPE inventory
Challenges Faced
Initial feed update timeout during setup
SSL certificate warning in browser
Understanding scan configurations and output
Outcome
Successfully performed vulnerability scanning using OpenVAS
Identified and analyzed system vulnerabilities
Gained practical knowledge of vulnerability assessment
Understood real-world security risks and mitigation techniques
Conclusion

The system was found to be mostly secure, with only one medium-level vulnerability related to SSL/TLS configuration. Implementing the recommended mitigation steps will further strengthen the system’s security posture.

Author

Chiranth S
