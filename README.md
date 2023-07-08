### credit_loan_predict
# Classification Model for Credit Loan Approval Predictions
Rakamin Final Project: Data Maestros - Data Science Batch 31

## Work Environment
- Tools: [Google Colab](https://colab.research.google.com/)
- Programming Language: Python
- Libraries
- Dataset: [Kaggle](https://www.kaggle.com/mirbektoktogaraev/should-this-loan-be-approved-or-denied)

## Script
Open in Colab
> [***Predicting Loan Approval using Machine Learning Model.ipynb***](https://colab.research.google.com/drive/1dB4Hf8jwmOlV3hmkmHmvmX5F9XKxhG-v?usp=sharing)

## Table of Content
- Business Understanding
  - Problem Statement
  - Roles
  - Goals
  - Objectives
  - Business Metrics
- Data Preparation
  - Data Description
- Data Understanding
  - Exploratory Data Analysis (EDA)
  - Business Insight
- Data Preprocessing
  - Handling Missing Values
  - Handling Duplicated Rows
  - Feature Extraction
  - Feature Encoding (Categorical -> Numerical)
  - Feature Selection
  - Data Splitting
  - Handling Outliers
  - Handling Imbalaced Data
- Machine Learning Model
- Recommendation

## Business Understanding
- Problem Statement

**Small Business Administration (SBA)** adalah sebuah perusahaan penjamin pinjaman yang berlokasi di US mengalami kerugian akibat banyaknya nasabah yang gagal bayar *(default)* dengan persentase mencapai 17,56%. 
- Roles

***Data Scientist Consultant*** berperan membantu perusahaan dalam melakukan **analisis permasalahan dan menganalisa potensi business development** berdasarkan data yang tersedia guna meningkatkan performa perusahaan.

- Goals

Perusahaan SBA ingin **menurunkan persentase nasabah yang berpotensi gagal bayar (default rate)** sehingga bisa meminimalisir resiko terjadinya kerugian yang besar.

- Objectives

1. Membangun ***model machine learning*** menggunakan *credit score automation,*
2. Menemukan faktor penting *(feature importance)* dan karakteristik nasabah yang layak mendapatkan pinjaman,
3. Memberikan **rekomendasi** yang akan meningkatkan efektivitas perusahaan dengan memberikan pinjaman kepada nasabah yang layak mendapatkan pinjaman.
   
- Business Metrics

***Persentase nasabah yang berpotensi gagal bayar (default rate)***

## Data Preparation
Deskripsi informasi atas fitur-fitur yang terdapat di dalam dataset:
- `LoanNr_ChkDgt` = Identifier Primary key
- `Name` = Borrower name
- `City` = Borrower city
- `State` = Borrower state
- `Zip` = Borrower zip code
- `Bank` = Bank name
- `BankState` = Bank state
- `NAICS` = North American industry classification system code
- `ApprovalDate` = Date SBA commitment issued
- `ApprovalFY` = Fiscal year of commitment
- `Term` = Loan term in months
- `NoEmp` = Number of business employees
- `NewExist` - 1 = Existing business (0), 2 = New business (1)
- `CreateJob` = Number of jobs created
- `RetainedJob` = Number of jobs retained
- `FranchiseCode` = Franchise code, (00000 or 00001) = No * franchise
- `UrbanRural` - 1 = Urban, 2 = Rural, 0 = undefined
- `RevLineCr` = Revolving line of credit: Y = Yes, N = No
- `LowDoc` = LowDoc Loan Program: Y = Yes, N = No
- `ChgOffDate` = The date when a loan is declared to be in * default
- `DisbursementDate` = Disbursement date
- `DisbursementGross` = Amount disbursed
- `BalanceGross` = Gross amount outstanding
- `MIS_Status` - Loan status charged off = CHGOFF (1), Paid in full = PIF (0)
- `ChgOffPrinGr` = Charged-off amount
- `GrAppv` = Gross amount of loan approved by bank
- `SBA_Appv` = SBA’s guaranteed amount of approved loan

Note: **`MIS_Status`** = Target Feature

## Data Understanding
### Basic Datasets Information
- Dataset terdiri dari `899.164 rows` dan `27 columns`
- Terdapat **17 data kategorik** dan **10 data numerik**
- Terdapat **11 fitur data null**

### Exploratory Data Analysis
- Univariate Analysis

Analisis setiap fitur menggunakan **boxplot dan histogram**

- Multivariate Analysis

Analisis antar-2-variabel berhubungan menggunakan **scatter plot dan heatmap** untuk melihat korelasi label-fitur
