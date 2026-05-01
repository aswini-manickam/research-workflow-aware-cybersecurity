[README_ICFACT.md](https://github.com/user-attachments/files/27272145/README_ICFACT.md)

#  Research Publication - Workflow-Aware Cybersecurity for Medical Radiology

> First-author conference paper presented at ICFACT-25 | Proceedings accepted for publication in Atlantis Press (Springer, Scopus-indexed) | Research conducted at C-DAC Kolkata - India's apex Government R&D institute for computing and cybersecurity.

[![Conference](https://img.shields.io/badge/Conference-ICFACT--25-blue?style=flat)](https://icfact.in/)
[![Publisher](https://img.shields.io/badge/Publisher-Atlantis%20Press%20%7C%20Springer-green?style=flat)](https://www.atlantis-press.com/)
[![Indexed](https://img.shields.io/badge/Indexed-Scopus-orange?style=flat)]()
[![Status](https://img.shields.io/badge/Status-Under%20Review-yellow?style=flat)]()
[![Affiliation](https://img.shields.io/badge/Affiliation-C--DAC%20Kolkata-darkblue?style=flat)](https://www.cdac.in/)

---

##  Paper Details

| Field | Details |
|-------|---------|
| **Title** | Workflow Aware Cybersecurity for Preventing Repeat Imaging in Medical Radiology |
| **Author** | Aswini Manickam *(First Author)* |
| **Conference** | International Conference on Advances in Forensics and Cyber Technologies (ICFACT-25) |
| **Venue** | Malla Reddy University, Hyderabad, India |
| **Publisher** | Atlantis Press (Springer) |
| **Indexing** | Scopus |
| **Status** | Proceedings accepted - publication forthcoming |
| **Research Institution** | C-DAC (Centre for Development of Advanced Computing), Kolkata |

>  **Full paper link will be added here once published by Atlantis Press / Springer.**

---

##  Abstract

Medical imaging workflows vary widely across regions and hospital systems, shaped by infrastructure maturity, pace of digital transformation, and the extent of cloud and AI integration. Hospitals face substantial barriers when transitioning to integrated operational and security workflows for imaging - including high upfront costs, legacy system incompatibilities, data privacy and cybersecurity concerns, staff resistance, limited trust in AI performance, and complex regulatory requirements.

Existing Picture Archiving and Communication Systems (PACS) security guidelines focus on technical controls and general risk reduction, but **do not explicitly link security events to measurable radiology workflow outcomes** such as repeat imaging rates, turnaround time, or scanner utilisation.

At present, to the authors' knowledge, **no cybersecurity architecture has been designed and evaluated with "repeat imaging rate" as a primary clinical performance metric** across both AI-enabled and legacy imaging systems.

### This study addresses that gap through two main contributions:

**1. FMEA/RPN-Based Cybersecurity Architecture**
A Failure Mode and Effects Analysis (FMEA) / Risk Priority Number (RPN) framework that directly links imaging-system security events - PACS logs, scanner status, AI inference logs - to measurable repeat imaging frequency via standardised repeat-scan failure modes (FM1-FM4) and RPN-weighted SOC playbooks.

**2. Laboratory Evaluation Across Imaging Workflow Types**
A simulation-based evaluation across legacy, cloud, and AI-augmented imaging workflows targeting:
- **30% reduction** in repeat imaging events
- **95% detection rate** of simulated cyberattacks

The proposed architecture integrates established **NIST controls** and **FMEA best practices** into a workflow-aware FMEA/RPN-to-SOC pipeline aimed at minimising avoidable repeat imaging.

---

##  Research Problem

### The Gap This Paper Addresses

Standard healthcare cybersecurity frameworks (NIST, HIPAA, PACS guidelines) are designed around data protection and access control. They answer: *"Is the system secure?"*

This research asks a different question: **"Does a security event cause a patient to be re-scanned?"**

Repeat imaging events carry real clinical and operational costs:
- Increased patient radiation exposure
- Scanner and staff resource waste
- Workflow delays and downstream scheduling impact
- Financial cost per repeat scan

By treating **repeat imaging rate** as the primary security performance metric, this architecture bridges the gap between SOC operations and clinical radiology outcomes — a connection that, to the authors' knowledge, had not previously been formalised in the literature.

---

##  Architecture Overview

```
Imaging System Events
├── PACS Logs              ← Archiving and retrieval anomalies
├── Scanner Status Feeds   ← Operational state and fault signals  
└── AI Inference Logs      ← AI-augmented workflow events
         │
         ▼
FMEA/RPN Analysis Engine
├── FM1 — [Repeat-scan failure mode 1]
├── FM2 — [Repeat-scan failure mode 2]
├── FM3 — [Repeat-scan failure mode 3]
└── FM4 — [Repeat-scan failure mode 4]
         │
   RPN Weighting
         │
         ▼
SOC Playbook Trigger
├── Alert prioritisation by clinical impact
├── Incident response mapped to repeat imaging risk
└── Workflow-aware escalation paths
         │
         ▼
Outcome Metrics
├── Repeat imaging rate reduction target: 30%
└── Attack detection rate target: 95%
```

---

##  Methodology

| Component | Approach |
|-----------|----------|
| **Risk Framework** | FMEA (Failure Mode and Effects Analysis) with RPN scoring |
| **Security Controls** | NIST Cybersecurity Framework controls |
| **Evaluation Method** | Laboratory simulation across 3 workflow types |
| **Workflow Types Tested** | Legacy imaging systems · Cloud-integrated · AI-augmented |
| **Primary Metric** | Repeat imaging rate (clinical outcome) |
| **Secondary Metric** | Cyberattack detection rate |
| **SOC Integration** | RPN-weighted playbooks mapped to clinical failure modes |

---

##  Research Domain Intersections

This paper sits at the intersection of three fields:

```
Healthcare Informatics          Cybersecurity Operations
       │                                │
       └──────────┬─────────────────────┘
                  │
         Medical Radiology
         Workflow Optimisation
```

**Key domain areas covered:**
- PACS (Picture Archiving and Communication Systems) security
- SOC operations in healthcare environments
- FMEA applied to cybersecurity architecture design
- AI-augmented vs legacy imaging system security posture
- Clinical outcome metrics as security KPIs
- NIST framework adaptation for radiology workflows

---

##  Research Context

This research was conducted during a internship at **C-DAC (Centre for Development of Advanced Computing), Kolkata** - the Government of India's apex R&D institute for advanced computing and cybersecurity.

C-DAC operates under the **Ministry of Electronics and Information Technology (MeitY)** and is India's primary government institution for cybersecurity research, high-performance computing, and digital infrastructure.

The research was presented at **ICFACT-25** (International Conference on Advances in Forensics and Cyber Technologies), with proceedings accepted for publication through **Atlantis Press (Springer)**, indexed in **Scopus**.

---

##  Research Interests

This publication reflects broader research interests in:

- **SOC automation** - reducing analyst burden through workflow-aware alerting
- **Digital forensics and incident investigation** - applied to healthcare environments
- **Healthcare cybersecurity** - bridging clinical operations and security operations
- **SIEM-based threat detection** - correlated with operational outcomes
- **FMEA-driven security architecture** - risk-quantified design methodologies
- **Cybersecurity pedagogy** - translating research into hands-on lab design

---

##  Key References & Frameworks

- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
- [NIST SP 800-66 - HIPAA Security Rule Guidance](https://csrc.nist.gov/publications/detail/sp/800-66/rev-2/final)
- [FMEA Methodology - ASQ](https://asq.org/quality-resources/fmea)
- [PACS Security - HIMSS](https://www.himss.org/)
- [Scopus - Atlantis Press](https://www.atlantis-press.com/)

---

##  Note on Full Paper Access

This repository contains only publicly presented material - the abstract and research overview as presented at ICFACT-25. The full manuscript is under review and will be linked here upon official publication by Atlantis Press (Springer).

If you are a researcher or reviewer seeking access to the full paper, please contact via [LinkedIn](https://linkedin.com/in/aswinimanickam).

---

##  Author

**Aswini Manickam** *(First Author)*
Cybersecurity Researcher | C-DAC Kolkata
[GitHub](https://github.com/aswinimanickam) · [LinkedIn](https://linkedin.com/in/aswinimanickam)

---

*Part of the [Cybersecurity Project Portfolio](https://github.com/aswinimanickam)*
