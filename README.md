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

Almost half of Medicaid spending is attributed to behavioral health conditions, including substance use disorders (SUD). Transgender and gender diverse people are disproportionally affected by overdose and SUD, including alcohol use, tobacco use, and other illicit drug use. As Medicaid expenditures for SUD treatment grows, it is increasingly important to understand the drivers of SUD treatment initiation among transgender patients in order to develop targeted strategies for treatment. This is the first study of SUD treatment among transgender Medicaid beneficiaries using insurance claims data from 2010 to 2020. We test differences in initiation and engagement with treatment between transgender and cisgender beneficiaries. Our primary hypothesis is that transgender beneficiaries had lower levels of initiation and treatment for SUD.

## Table of Contents
- [Project Description](#project-description)
- [Requirements](#requirements)
- [Table of contents](#table-of-contents)
- [Requirements](#requirements)
- [Producing Data](#producing-data)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Machine Learning](#machine-learning)

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

## Producing Data 
[(Back to top)](#table-of-contents)

[This code](trans_sud_clean.ipynb) produces the data using the available files, and creating additional variables with our user-created dictionaries. 

- Available files
  - Claims (`arp120.claims`)
  - Enrollment (`arp120.mem_detail`)
  - [CDPS risk score](https://www.cms.gov/Research-Statistics-Data-and-Systems/Research/HealthCareFinancingReview/List-of-Past-Articles-Items/CMS1191627) (`arp120.cdps`)
  - [Initiation and Engagement with Treatment HEDIS Measures](https://www.ncqa.org/hedis/measures/initiation-and-engagement-of-alcohol-and-other-drug-abuse-or-dependence-treatment/) (`arp120.j_iet_mem`)
  
- User-created data
  - Transgender Dx
  - Chronic Pain Dx
  - Substance Use Disorder Dx
  - Severe Mental Health Dx

## Exploratory Data Analysis
[(Back to top)](#table-of-contents)

[This code](trans_sud_eda.ipynb) investigates the quality and structure of the data, and produces visualizations.

- Descriptive Statistics
- Data Visualization
- Logistic Regression

## Machine Learning
[(Back to top)](#table-of-contents)

[This code](trans_sud_ml.ipynb) presents models to predict SUD treatment.

- Data pre-processing
- Split into test and training sets
- Build Models
- Evaluate
- Finalize

## Funding & Collaborators

This project is funded by a [K01 grant](https://reporter.nih.gov/search/TwUZdye2PkK94TZ0KQCM5A/project-details/10432100) from the National Institute on Drug Abuse.

Data and support are provided by [The Center for Health Systems Effectiveness](https://www.ohsu.edu/center-for-health-systems-effectiveness) at OHSU.
