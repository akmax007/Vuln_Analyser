# Vulnerability Management Dashboard

A Python-based Vulnerability Management Dashboard built using Streamlit that helps security teams analyze vulnerability scan reports, enrich CVE data, and generate remediation recommendations.

## Features

- Upload vulnerability scan reports in Excel format
- Analyze Critical, High, Medium, and Low vulnerabilities
- Visualize severity distribution
- Identify top recurring vulnerabilities
- Retrieve CVE details from the NVD (National Vulnerability Database)
- Display CVSS scores and severity ratings
- Generate remediation recommendations
- Export CVE and remediation reports
- Interactive web dashboard

---

## Dashboard Screens

### Upload Vulnerability Report
Upload Excel-based vulnerability scan reports for analysis.

### Severity Distribution
Visual representation of vulnerabilities categorized by severity.

### Top Vulnerabilities
Identify the most frequently occurring vulnerabilities.

### CVE Analysis
Retrieve:
- CVSS Score
- Severity
- Description
- CVE Details

### Remediation Recommendations
Provides actionable recommendations to mitigate identified vulnerabilities.

---

## Tech Stack

### Frontend
- Streamlit

### Backend
- Python

### Libraries
- Pandas
- OpenPyXL
- Requests
- Collections

### Data Sources
- Excel Vulnerability Reports
- NVD API

---

## Project Structure

```text
project/
│
├── app.py
├── requirements.txt
├── sample_data/
│   └── vulnerability_scan.xlsx
│
├── reports/
│   ├── cve_report.csv
│   └── remediation_report.csv
│
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/akmax007/Vuln_Analyser.git
cd vulnerability-management-dashboard
```

Install dependencies:

```bash
pip install streamlit pandas openpyxl requests
```

Run the application:

```bash
streamlit run main.py
```

Open your browser:

```text
http://localhost:8501
```

---

## Sample Input Format

| Host | IP | Severity | Name | CVE | Plugin_ID | Description |
|--------|--------|--------|--------|--------|--------|--------|
| WEB01 | 10.0.1.10 | Critical | Apache Log4j RCE | CVE-2021-44228 | 156001 | Log4j vulnerability |

---

## Workflow

```text
Excel Upload
      ↓
Pandas Processing
      ↓
Severity Analysis
      ↓
CVE Lookup (NVD API)
      ↓
Remediation Engine
      ↓
Dashboard Visualization
      ↓
CSV Report Export
```

---

## Future Enhancements

- AI-powered remediation generation
- Automatic patch lookup
- PDF report generation
- Email notifications
- Snowflake integration
- Vulnerability trend analysis
- Asset risk scoring
- CISA KEV integration

---

## Use Cases

- Vulnerability Assessment
- Security Operations (SOC)
- Vulnerability Management Teams
- Compliance Reporting
- Security Audits
- Cybersecurity Training Projects

---

## Author

Ankit Bewal

Cybersecurity | Data Engineering | Automation

