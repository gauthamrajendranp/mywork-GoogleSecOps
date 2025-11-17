YARA-L Detection Rules for Google SecOps

A comprehensive collection of YARA-L detection rules designed for Google Chronicle SIEM (SecOps) to enhance security monitoring across various cloud environments and use cases.

📋 Overview
This repository contains custom YARA-L detection rules developed for proactive threat detection and security monitoring in Google Chronicle. These rules cover multiple security domains including Office 365, cloud infrastructure (AWS, GCP), geo-blocking scenarios, and other critical security use cases.

🚀 Use Cases Covered

* Office 365 Security
    1. Suspicious login patterns and impossible travel
    2. Mass file download and sharing activities
    3. Malicious Power Automate flows
    4. Unusual mailbox access and forwarding rules

* GCP Security Monitoring
    1. Suspicious Compute Engine instance creation
    2. IAM privilege escalation attempts
    3. Cloud Storage bucket enumeration
    4. Cryptocurrency mining detection

* AWS Security Monitoring
    1. Unusual CloudTrail events and API calls
    2. Security group modifications
    3. Unauthorized resource access
    4. Root account usage monitoring

* Geo-Blocking & Location-based Detection
    1. Access from high-risk countries
    2. VPN and proxy service detection
    3. Data exfiltration to suspicious locations
    4. Geographic anomaly detection

*  Network Security
    1. Port scanning and reconnaissance
    2. Brute force authentication attempts
    3. DNS tunneling detection
    4. Suspicious network traffic patterns

🛠️ Getting Started
  * Prerequisites
    1. Google Chronicle SIEM instance
    2. Appropriate data ingestion configured
    3. Required permissions to create and deploy detection rules

Installation
  1. Clone this repository:
        bash
        git clone https://github.com/your-username/yara-l-detection-rules.git
        cd yara-l-detection-rules
  2. Review and customize rules according to your environment
  3. Deploy rules to your Google Chronicle instance

Rule Deployment
Refer to the Deployment Guide for detailed instructions on:
  1. Rule validation and testing
  2. Deployment best practices
  3. Rule tuning and customization

📝 Rule Development
Template Usage:
Use the provided rule template for creating new detection rules:

    yara-l
    rule rule_name {
    meta:
    author = "Your Name"
    description = "Brief description of the rule"
    severity = "MEDIUM"
    confidence = "HIGH"
    use_case = "Specific use case"

    events:
    // Event matching conditions

    match:
    // Aggregation fields

    condition:
    // Rule conditions
    }

Testing:
  1. Use test cases in the tests/ directory
  2. Validate rules with sample data
  3. Test rule performance and accuracy

🔧 Configuration
Customization:
  1. Update rule thresholds based on your environment
  2. Modify watchlists and reference data
  3. Adjust severity levels according to your risk appetite
  4. Customize notification channels

Tuning Recommendations
  1. Start with higher thresholds and adjust downward
  2. Monitor false positive rates
  3. Regularly review and update rules
  4. Consider your organization's specific risk profile

📊 Monitoring & Maintenance
Rule Performance:
  1. Monitor rule execution logs
  2. Track detection rates and false positives
  3. Review rule effectiveness regularly

Updates
  1. Regularly update rules for new threats
  2. Incorporate new data sources
  3. Adjust for changes in your environment

🤝 Contributing
I welcome contributions! Please see our Contributing Guidelines for details on:

  1. Submitting new detection rules
  2. Reporting issues
  3. Improving existing rules
  4. Code review process

⚠️ Disclaimer
These detection rules are provided as-is and should be thoroughly tested in your environment before deployment in production. The author is not responsible for any false positives, missed detections, or other issues that may arise from using these rules.

📞 Support
For questions or issues:

  1. Check the troubleshooting guide
  2. Review existing GitHub issues
  3. Create a new issue with detailed information

🔒 Security Considerations
  1. Regularly review and update detection logic
  2. Monitor for rule evasion techniques
  3. Keep rules aligned with your security policies
  4. Conduct regular threat hunting exercises

Maintained by: Gowthaman | Security Engineer
Last Updated: November 17, 2025

This response is AI-generated, for reference only.
