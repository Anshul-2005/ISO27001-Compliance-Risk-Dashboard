# ISO 27001 Compliance & Risk Dashboard

A portfolio project demonstrating an end-to-end **ISO/IEC 27001
compliance, control-gap, information-security risk, and remediation
analysis workflow** using Microsoft Excel and Power BI.

> **Portfolio disclaimer:** This is a simulated assessment created for
> portfolio/learning purposes. The organization, assessment records,
> control evidence references, risks, and remediation records are not
> presented as a real certification audit or as evidence of an actual
> organization's ISO/IEC 27001 certification status.

## Project Overview

The project models how a GRC / Information Security Compliance analyst
could organize assessment evidence, evaluate control implementation,
maintain a risk register, track remediation, and present
management-level findings through an interactive Power BI dashboard.

### Tools

-   Microsoft Excel --- assessment data, control register, gap
    assessment, risk register and remediation tracker
-   Power BI Desktop --- data model, DAX measures, interactive dashboard
    and visual analysis
-   ISO/IEC 27001 control framework concepts --- control assessment and
    information-security risk management
-   DAX --- compliance and risk calculations, including the Likelihood ×
    Impact risk concentration matrix

## Dashboard Structure

### 1. Executive Compliance Overview

Provides a management-level view of:

-   Overall compliance score
-   Total controls
-   Implemented controls
-   Partially implemented controls
-   Not implemented controls
-   Total risks
-   Critical and high risks
-   Remediation activity
-   Average remediation completion

### 2. Control & Gap Analysis

Provides control-level analysis using:

-   Status filter
-   Control category filter
-   Priority filter
-   Compliance by control category
-   Control status distribution
-   Detailed control/gap register

### 3. Risk Analysis

Provides risk-level analysis using:

-   Inherent risk-level filter
-   Asset filter
-   Likelihood × Impact risk concentration matrix
-   Detailed risk register

The matrix uses disconnected 1--5 Likelihood and Impact axis tables and
a DAX measure to count risks at each combination.

### 4. Remediation Analysis

Provides remediation-focused analysis using:

-   Priority filter
-   Status filter
-   Remediation status distribution
-   Average completion by priority
-   Detailed remediation tracker

## Source Data Model

The Excel workbook contains the assessment data used to build the Power
BI model, including:

-   `ControlMaster`
-   `GapAssessment`
-   `Risk_Register`
-   `Remediation_Tracker`
-   `Evidence_Index`
-   `Management_Summary`

The Power BI semantic model connects the assessment tables through their
relevant identifiers and uses DAX measures for dashboard calculations.

## Key Portfolio Findings

The simulated assessment currently shows:

  Metric                             Result
  -------------------------------- --------
  Total controls                         40
  Implemented controls                   18
  Partially implemented controls         20
  Not implemented controls                2
  Overall compliance score            70.0%
  Total risks                            13
  Critical risks                          6
  High risks                              7
  Remediation actions                    13
  Average remediation completion      15.4%

These values are portfolio-simulation results and should not be
interpreted as an actual organization's compliance status.

## Risk Methodology

The project uses a basic likelihood-impact approach:

**Inherent Risk Score = Likelihood × Impact**

Likelihood and Impact are represented on a 1--5 scale.

The dashboard separates:

-   Inherent risk --- exposure before treatment
-   Residual risk --- remaining exposure after treatment

The risk concentration matrix shows the number of risks occupying each
Likelihood × Impact combination.

## Compliance Assessment Approach

Controls are assessed using implementation states such as:

-   Implemented
-   Partially Implemented
-   Not Implemented

The portfolio compliance score is calculated using weighted
implementation status:

-   Implemented = 100%
-   Partially Implemented = 50%
-   Not Implemented = 0%

Therefore:

**Compliance Score = (Implemented + 0.5 × Partially Implemented) / Total
Controls × 100**

For this assessment:

**(18 + 0.5 × 20) / 40 × 100 = 70%**

## Repository Structure

``` text

ISO27001-Compliance-Risk-Dashboard/
│
├── dashboard/
│   └── ISO27001_Compliance_Risk_Dashboard.pbix
│
├── data/
│   └── ISO27001_Compliance_Assessment.xlsx
│
├── docs/
│   └── ISO27001_Compliance_Gap_Assessment_Explanation.docx
│
├── screenshots/
│   ├── executive-compliance-overview.png
│   ├── control-gap-analysis.png
│   ├── risk-analysis.png
│   └── remediation-analysis.png
│
├── .gitignore
└── README.md
```

## How to Use

1.  Download the `.pbix` file.
2.  Open it with Microsoft Power BI Desktop.
3.  If Power BI requests the Excel source, point it to the included
    workbook.
4.  Use the four report pages and slicers to explore the assessment.
5.  Review the Excel workbook to understand the underlying assessment
    records.

## Skills Demonstrated

-   GRC / Information Security Compliance
-   ISO/IEC 27001 control assessment concepts
-   Control-gap analysis
-   Risk identification and risk scoring
-   Inherent vs. residual risk analysis
-   Risk register management
-   Remediation tracking
-   Evidence tracking
-   Excel-based compliance data management
-   Power BI data modeling
-   DAX measures
-   Interactive dashboard development
-   Management reporting and data visualization

## Important Note

This project demonstrates the **workflow and analytical thinking**
expected in an entry-level GRC / Information Security Compliance role.
It is not a substitute for an organization's formal ISMS audit,
certification audit, statement of applicability, risk acceptance
process, or independent audit evidence.
