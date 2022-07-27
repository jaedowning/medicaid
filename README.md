![](./images/ohp_banner.png)

<p align="center">
  <sub>
    Built with ❤︎ by
    <a href="https://github.com/jaedowning">Jae</a>, 
    and the community!
  </sub>
</p>

# Substance Use Treatment

## Project Description

Almost half of Medicaid spending is attributed to behavioral health conditions, including substance use disorders (SUD). Transgender and gender diverse people are disproportionally affected by overdose and SUD, including alcohol use, tobacco use, and other illicit drug use. As Medicaid expenditures for SUD treatment grows, it is increasingly important to understand the drivers of initiation and treatment of SUD among transgender patients in order to develop targeted strategies for treatment. This first study of SUD treatment among transgender Medicaid beneficiaries using insurance claims data from 2010 to 2020. We provide insights into similiaries and differences in initiation and engagement with treatment between transgender and cisgender beneficiaries. Our primary hypothesis is that transgender beneficiaries had lower levels of initiation and treatment for SUD.

## Table of Contents
- [Project Description](#project-description)
- [Table of contents](#table-of-contents)
- [Requirements](#requirements)
- [Data](#data)


## Requirements
[(Back to top)](#table-of-contents)

* **Python 3.9+**
* **NumPy (`pip install numpy`)**
* **Pandas (`pip install pandas`)**
* **Scikit-learn (`pip install scikit-learn`)**
* **SciPy (`pip install scipy`)**
* **MatplotLib (`pip install matplotlib`)**
* **Seaborn (`pip install seaborn`)**
* **TableOne (`pip install tableone`)**
* **Sqlite3 (`pip install sqlite3`)**
* **SQLAlcemy (`pip install SQLAlchemy`)**
* **Psycopg (`pip install psycopg2`)**

## Data 

- Existing Data on Server
  - Claims (`arp120.claims`)
  - Enrollment (`arp120.mem_detail`)
  - [CDPS risk score](https://www.cms.gov/Research-Statistics-Data-and-Systems/Research/HealthCareFinancingReview/List-of-Past-Articles-Items/CMS1191627) (`arp120.cdps`)
  - [Initiation and Engagement with Treatment HEDIS Measures](https://www.ncqa.org/hedis/measures/initiation-and-engagement-of-alcohol-and-other-drug-abuse-or-dependence-treatment/) (`arp120.j_iet_mem`)
  
- User Created Data
  - Transgender Dx
  - Chronic Pain Dx
  - Substance Use Disorder Dx
  - Severe Mental Health Dx

## Approach

- Data wrangling
- Data visualization
- Modeling
  - Logistic regression
  - Oaxaca Blinder
  - Machine Learning
- Curation for publication

