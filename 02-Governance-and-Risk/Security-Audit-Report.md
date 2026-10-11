# Botium Toys: Scope, Goals, and Risk Assessment Report

> [!NOTE]
> **Portfolio Project Disclaimer:**  
> This project was completed as part of the **Google Cybersecurity Professional Certificate**. "Botium Toys" is a fictional company scenario used for educational and assessment purposes. All data, findings, and recommendations presented here are simulated and intended solely to demonstrate practical knowledge in security audits, risk assessment, and compliance frameworks.

## Scope and Goals of the Audit

* **Scope:** The scope of this audit is defined as the entire security program at Botium Toys. This includes their assets like employee equipment and devices, their internal network, and their systems. You will need to review the assets Botium Toys has and the controls and compliance practices they have in place.
* **Goals:** Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices that need to be implemented to improve Botium Toys’ security posture.

---

## Current Assets

Assets managed by the IT Department include:
* On-premises equipment for in-office business needs
* Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
* Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse
* Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
* Internet access
* Internal network
* Data retention and storage
* Legacy system maintenance: end-of-life systems that require human monitoring

---

## Risk Assessment

### Risk Description
Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards.

### Control Best Practices
The first of the five functions of the NIST CSF is **Identify**. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.

### Risk Score
On a scale of 1 to 10, the risk score is **8**, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.

### Additional Comments
The potential impact from the loss of an asset is rated as **medium**, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is **high** because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Specific findings include:

* Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.
* Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database.
* Access controls pertaining to least privilege and separation of duties have not been implemented.
* The IT department has ensured availability and integrated controls to ensure data integrity.
* The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.
* Antivirus software is installed and monitored regularly by the IT department.
* The IT department has not installed an intrusion detection system (IDS).
* There are no disaster recovery plans currently in place, and the company does not have backups of critical data.
* The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.
* Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters).
* There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.
* While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.
* The store’s physical location, which includes Botium Toys’ main offices, storefront, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.

---

## Controls and Compliance Checklist

### Administrative Controls

| Control Name | Control Type and Explanation | Needs to be Implemented (X) | Priority |
| :--- | :--- | :---: | :---: |
| **Least Privilege** | Preventative; Reduce risk and overall impact of malicious insider or compromised accounts | X | High |
| **Disaster recovery plans** | Corrective; Provide business continuity | X | High |
| **Password policies** | Preventative; Establish password strength rules to improve security/reduce likelihood of account compromise through brute force or dictionary attack techniques | X | High |
| **Separation of duties** | Preventative; Reduce risk and overall impact of malicious insider or compromised accounts | X | High |

### Technical Controls

| Control Name | Control Type and Explanation | Needs to be Implemented (X) | Priority |
| :--- | :--- | :---: | :---: |
| **Firewall** | Preventative; To filter unwanted or malicious traffic from entering the network | Implemented | — |
| **Intrusion detection system (IDS)** | Detective; To detect and prevent anomalous traffic that matches a signature or rule | X | High |
| **Backups** | Corrective; Restore/recover from an event | X | High |
| **Password management system** | Preventative; Reduce password fatigue | X | High |
| **Antivirus software** | Preventative; Scans to detect and quarantine known threats | Implemented | — |
| **Manual monitoring, maintenance, and intervention for legacy systems** | Preventative; Necessary to identify and manage threats, risks, or vulnerabilities to out-of-date systems | X | High |
| **Encryption** | Deterrent; Provide confidentiality to sensitive information | X | High |

### Physical Controls

| Control Name | Control Type and Explanation | Needs to be Implemented (X) | Priority |
| :--- | :--- | :---: | :---: |
| **Time-controlled safe** | Deterrent; Reduce attack surface and overall impact from physical threats | X | Medium |
| **Adequate lighting** | Deterrent; Deter threats by limiting “hiding” places | X | Low |
| **Locks (offices, storefront, warehouse)** | Deterrent/Preventative; Bolster integrity by deterring and preventing unauthorized personnel/individuals from physically accessing assets | Implemented | — |
| **Closed-circuit television (CCTV) surveillance** | Preventative/Detective; Can reduce risk of certain types of events occurring and can be used after an event to inform on conditions | Implemented | — |
| **Locking cabinets (for network gear)** | Preventative; Bolster integrity by preventing unauthorized personnel and other individuals from physically accessing or modifying network infrastructure gear | X | Medium |
| **Signage indicating alarm service provider** | Deterrent; Deter certain types of threats by making the likelihood of a successful attack seem low | X | Medium |
| **Fire detection/prevention (fire alarm, sprinkler system, etc.)** | Detective/Preventative; Detect fire in physical location and prevent damage to physical assets such as inventory, servers, etc. | Implemented | — |

---

## Compliance Checklist

### Payment Card Industry Data Security Standard (PCI DSS)

| Yes | No | Best Practice |
| :---: | :---: | :--- |
| | X | Only authorized users have access to customers’ credit card information. |
| | X | Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment. |
| | X | Implement data encryption procedures to better secure credit card transaction touchpoints and data. |
| | X | Adopt secure password management policies. |

### General Data Protection Regulation (GDPR)

| Yes | No | Best Practice |
| :---: | :---: | :--- |
| | X | E.U. customers’ data is kept private/secured. |
| X | | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. |
| | X | Ensure data is properly classified and inventoried. |
| | X | Enforce privacy policies, procedures, and processes to properly document and maintain data. |

### System and Organization Controls (SOC Type 1, SOC Type 2)

| Yes | No | Best Practice |
| :---: | :---: | :--- |
| | X | User access policies are established. |
| | X | Sensitive data (PII/SPII) is confidential/private. |
| X | | Data integrity ensures the data is consistent, complete, accurate, and has been validated. |
| X | | Data is available to individuals authorized to access it. |

---

## Recommendations

Because Botium Toys has business dealings with customers in the EU, it is imperative that the company first places a high priority on implementing control measures for best practices under **PCI DSS** and **GDPR**. Fines related to breaches of standards and regulations can result in catastrophic financial losses during an external audit.

The next recommended step is to strengthen Botium Toys’ security posture by completing all remaining required controls under the **Controls Assessment Checklist** in order of priority from **High to Low**.

These two key adjustments will ensure Botium Toys is sufficiently protected and prepared to manage the added security risks of local and overseas expansion while maintaining international regulatory compliance.
