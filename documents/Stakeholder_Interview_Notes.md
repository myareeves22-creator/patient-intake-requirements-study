# Stakeholder Interview Notes: Clinic Intake Operations

**Project Name:** Automated Patient Intake & Insurance Verification System  
**Date:** October 2026  
**Interviewer:** Business Analyst  
**Interviewees:** 
- Sarah Jenkins (Front Desk Operations Lead)
- Marcus Vance (Billing & Revenue Cycle Manager)

---

### Executive Context
The clinic network is experiencing lobby congestion during peak morning hours (8:00 AM – 10:30 AM) and an unsustainable rate of initial insurance claim rejections. This discovery session was conducted to identify front-line operational bottlenecks.

---

### Key Findings by Stakeholder

#### 1. Front Desk Operations (Sarah Jenkins)
* **Current Workflow:** Patients complete paper intake clipboards upon arrival. Receptionists manually re-key demographic and insurance details into the Electronic Health Record (EHR) system while the patient waits at the window.
* **Pain Points:**
  * Average paper intake takes 10–15 minutes per patient.
  * Manual data entry leads to frequent typos in patient names, birth dates, and policy IDs.
  * Front-desk staff feel rushed, causing patient frustration and lobby overcrowding.

#### 2. Billing & Revenue Cycle (Marcus Vance)
* **Current Workflow:** Claims are generated automatically from EHR data post-visit and sent to payers.
* **Pain Points:**
  * Approximately 18% of initial claims are rejected due to invalid policy numbers or inactive patient coverage.
  * Staff spend roughly 15 hours per week manually calling insurance carriers to verify coverage after appointments have already occurred.
  * Lack of upfront verification forces the clinic to bill patients directly after the fact, increasing uncollectible debt.

---

### Summary of High-Level Business Needs
1. Implement a digital pre-registration option accessible on mobile devices prior to clinic arrival.
2. Institute automated front-end data validation rules (e.g., mandatory field formatting for policy numbers).
3. Connect intake forms to real-time insurance payer APIs to flag inactive coverage at or before check-in.
