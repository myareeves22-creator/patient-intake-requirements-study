# Business Requirements Document (BRD)

**Project Name:** Automated Patient Digital Intake & Insurance Verification System  
**Document Version:** 1.0  
**Author:** Business Analyst  
**Date:** October 2026  

---

## 1. Executive Summary & Project Purpose
The primary objective of this project is to digitize and automate the clinic network's patient registration and insurance verification workflows. Replacing manual paper intake with a mobile pre-registration portal will decrease waiting room check-in times, streamline data entry into the EHR, and reduce front-end claim rejections.

---

## 2. Business Objectives & Success Metrics
* **Reduce Intake Processing Time:** Decrease average patient check-in cycle time from 15 minutes to under 4 minutes.
* **Decrease Claim Denials:** Reduce insurance claim rejections stemming from invalid demographic or policy data by 30% within 90 days post-implementation.
* **Operational Staff Savings:** Save an estimated 12 to 15 hours per week of manual data re-entry and verification calls across front-desk staff.

---

## 3. Stakeholder Matrix

| Stakeholder Group | Primary Interest / Role | Project Impact |
| :--- | :--- | :--- |
| **Front Desk Staff** | Primary users managing patient check-ins and lobby workflow. | High |
| **Billing & Revenue Team** | Downstream beneficiaries of accurate insurance data and pre-verified coverage. | High |
| **IT & Systems Lead** | Engineering lead oversight for EHR API integration and security protocols. | High |
| **Patients** | End users completing digital registration forms prior to visits. | High |

---

## 4. Functional Requirements (FR)

* **FR-01 (Automated Link Dispatch):** The system shall automatically send a secure, unique digital intake link to the patient via SMS and Email 48 hours prior to their scheduled appointment.
* **FR-02 (Field Validation Rules):** The digital form interface must enforce formatting constraints (regex patterns) on all mandatory fields including Name, DOB, Phone Number, and Insurance Policy ID.
* **FR-03 (Automated EHR Integration):** Completed intake responses must write directly to the clinic EHR database without requiring manual staff keying.
* **FR-04 (Payer API Verification):** Upon form submission, the system shall execute an automated query to the payer API to check real-time insurance eligibility.
* **FR-05 (Dashboard Flagging):** The front-desk system interface must display visual status indicators (Active, Inactive, Verification Error) for every scheduled patient.

---

## 5. Non-Functional Requirements (NFR)

* **NFR-01 (Security & Compliance):** System architecture and data transmission must strictly adhere to HIPAA regulations, using end-to-end AES 256-bit encryption for all Patient Health Information (PHI).
* **NFR-02 (System Latency):** Mobile web application pages must load in under 2 seconds on standard mobile networks (4G/5G).
* **NFR-03 (Usability & Accessibility):** Web interface must comply with WCAG 2.1 Level AA standards, offering high-contrast modes, minimum 16pt font options, and compatibility with mobile screen readers.
* **NFR-04 (Availability):** The digital registration portal must maintain 99.9% operational uptime.
