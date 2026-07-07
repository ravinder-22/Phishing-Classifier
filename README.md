# Phishing Website Detection Using Machine Learning

A machine learning project that detects phishing websites by analyzing URL-based, domain-based, and content-based features, helping protect users from scams, financial loss, and identity theft.

## Table of Contents

- [Overview](#overview)
- [Why This Matters](#why-this-matters)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Data Preprocessing](#data-preprocessing)
- [Models Used](#models-used)
- [Model Evaluation](#model-evaluation)
- [Deployment](#deployment)
- [Tech Stack](#tech-stack)
- [Results](#results)
- [Future Scope & Improvements](#future-scope--improvements)
- [Conclusion](#conclusion)

## Overview

Phishing is a cyber-attack where fraudulent websites steal sensitive information such as login credentials, banking details, and personal data. Traditional blacklist-based detection methods fail to catch new, previously unseen phishing sites.

This project uses **Machine Learning** to automate phishing detection by analyzing website features and classifying URLs as either **phishing** or **legitimate**.

## Why This Matters

- Protects users from scams, financial loss, and identity theft
- Automates detection instead of relying on manually maintained blacklists
- Adapts to new and evolving phishing techniques through feature-based analysis

## Dataset

- Contains **30 features** extracted from websites
- **Label**: `Result` → `-1` for phishing, `1` for legitimate

**Feature categories:**

| Category | Examples |
|---|---|
| URL-based | Having IP Address, URL Length, Shortening Service |
| Domain-based | SSL State, Domain Registration Length |
| Content-based | Request URL, Links in Tags, Iframes |

## Project Workflow

1. Introduction
2. Environment Setup
3. Dataset Exploration
4. Data Preprocessing
5. Feature Engineering
6. Model Training & Evaluation
7. FastAPI Deployment
8. Docker
9. Cloud Deployment
10. CI/CD with GitHub Actions
11. Terraform Infrastructure
12. Final Wrap-Up

## Data Preprocessing

- Handling missing values
- Converting categorical data
- Normalizing feature values
- Splitting data into training and testing sets

## Models Used

The following classification models were trained and compared using **Scikit-learn**:

- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- Gradient Boosting (XGBoost)

## Model Evaluation

Model performance was assessed using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix** (to analyze false positives/negatives)

## Deployment

- Backend API built with **Flask** or **FastAPI**
- Connected to a front-end UI
- Hosted on cloud platforms (**AWS / Azure / GCP**)
- Containerized using **Docker**
- Infrastructure managed with **Terraform**
- Automated with **CI/CD via GitHub Actions**

## Tech Stack

- **Language**: Python
- **ML Libraries**: Scikit-learn, XGBoost
- **API Framework**: Flask / FastAPI
- **Containerization**: Docker
- **Infrastructure as Code**: Terraform
- **CI/CD**: GitHub Actions
- **Cloud**: AWS / Azure / GCP

## Results

- ML models successfully detect phishing websites with high accuracy
- **Random Forest** and **XGBoost** performed the best among the tested models
- Evaluation metrics (accuracy, precision, recall, F1-score) confirm strong model reliability

## Future Scope & Improvements

1. **Real-time Phishing Detection** — Integrate live URL scanning using API-based lookups instead of relying only on pre-collected datasets.
2. **Deep Learning for Enhanced Accuracy** — Use neural networks (LSTMs, CNNs) to capture hidden patterns in URLs and webpage content.
3. **Browser Extension for Phishing Prevention** — Build a Chrome/Firefox extension that dynamically analyzes URLs via the ML model API and warns users.
4. **Expanding Features for Better Detection** — Add NLP-based analysis of webpage text to catch urgency-based phishing language (e.g., "Your account will be blocked soon! Click here now!").
5. **Integration with Cybersecurity Systems** — Collaborate with email security solutions and build an AI-powered firewall to automatically block phishing domains.
6. **Improving Dataset Quality** — Continuously collect real-world phishing websites and use web scrapers to keep the dataset up to date.

## Conclusion

Phishing attacks are a growing cybersecurity threat, and traditional blacklist-based methods struggle to keep up with new attack patterns. By analyzing URL-based, domain-based, and content-based features, this project demonstrates that Machine Learning — particularly Random Forest and XGBoost — can classify phishing websites with high accuracy, helping automate detection and improve overall security.

---

*
