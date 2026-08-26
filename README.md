# Blue Team Capstone

## Project Overview

This project is a Blue Team cybersecurity capstone focused on vulnerability assessment, risk evaluation, and remediation.

The assessment focuses on **CVE-2009-0658**, a vulnerability affecting Adobe Acrobat and Reader. The goal of the project was to evaluate the vulnerability using the **CVSS v3.1 framework** and translate the findings into practical defensive recommendations.

## Objectives

- Assess a real-world vulnerability using CVSS v3.1.
- Evaluate the vulnerability from a defensive and risk-management perspective.
- Document the reasoning behind the CVSS scores.
- Develop practical remediation recommendations.
- Support the assessment with relevant research and evidence.

## What I Did

- Researched CVE-2009-0658 and its associated exploitation information.
- Performed Base, Temporal, and Environmental CVSS assessments.
- Documented the metric selections and scoring rationale.
- Reviewed publicly available proof-of-concept information.
- Developed remediation recommendations based on the assessment.
- Collected and documented supporting references.

## Assessment Results

| Assessment | Score |
|---|---:|
| Base Score | **7.8 (High)** |
| Temporal Score | **7.5 (High)** |
| Environmental Score | **7.5 (High)** |

The detailed scoring methodology, metric selection, and supporting evidence can be found in the [CVSS Assessment](cvss-assessment/) section.

## Project Structure

```text
blue-team-capstone/
│
├── cvss-assessment/
│   ├── overview.md
│   ├── base-score.md
│   ├── temporal-score.md
│   ├── environmental-score.md
│   └── screenshots/
│
├── recommendations/
│   └── remediation.md
│
├── references/
│   └── references.md
│
└── README.md 
```

## CVSS Assessment
Contains the detailed Base, Temporal, and Environmental score calculations, including the reasoning behind each metric selection and supporting screenshots.

## Recommendations
Contains the defensive recommendations developed from the assessment findings.

## References
Contains the vulnerability records, vendor advisory, exploitation references, and CVSS resources used during the assessment.

## Scope
This project focuses on vulnerability assessment and defensive analysis. The assessment uses publicly available information and does not involve testing against real-world systems or networks.
