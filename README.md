# 🌍 Too Good To Go: Enterprise Data Strategy & Architecture

## 📌 Project Overview
This repository contains a comprehensive enterprise data strategy and architectural framework developed for **Too Good To Go**, the world's leading food-waste reduction platform. 

The primary objective of this project is to address the data engineering and governance challenges associated with capturing, synchronising, and standardising partner data at scale. By designing a robust data infrastructure, this framework ensures real-time inventory accuracy across 150,000+ independent partner stores, preventing double-bookings and improving demand forecasting.

*This project was completed as part of the MSc in Data Analytics for Business at KEDGE Business School.*

---

## 🏗️ Core Architecture & Conceptual Data Model

Ingesting transaction data from dozens of different Point-of-Sale (POS) systems into a single clean schema is a major engineering challenge. To solve this, we designed a **Conceptual Data Model (Star Schema)**.

This schema normalises the data ecosystem by linking critical dimension tables (Customers, Partners, Products, Dates) with central fact tables capturing:
* Real-time inventory and reserved quantities.
* Order transactions and payment statuses.
* Environmental impact metrics (CO₂ saved, water saved).

![Conceptual Data Model](./assets/CDM_2.png)
*(Fig 1: The Star Schema linking dimensions and fact tables to support enterprise reporting and real-time operations.)*

---

## 📊 Business Intelligence & KPI Dashboard

To provide leadership with a single source of truth, we developed a **KPI Performance Dashboard**. This dashboard tracks the 10 most critical metrics across consumer engagement, financial results, and sustainability impact.

Key metrics tracked include:
* **Growth:** Weekly Active Users (WAU), Surprise Bags Sold, New Partner Sign-ups.
* **Retention:** Customer Retention Rate, Avg Partner Rating.
* **Impact:** Cumulative Meals Saved, CO₂ Avoided (Tonnes).

![KPI Dashboard](./assets/Dashboard_1.png)
*(Fig 2: FY 2024 KPI Performance Dashboard visualising momentum and growth trends.)*

---

## 📋 KPI Distribution Framework

Data is only valuable if it reaches the right stakeholders at the right time. We mapped a complete **KPI Distribution Matrix** to govern how these metrics are shared across the organisation. 

This matrix dictates the frequency, distribution channel, ownership, and strategic objective for every KPI. For example, the Head of Sustainability owns the monthly reporting of CO₂ saved to ensure public and NGO transparency, while the Head of Product monitors Weekly Active Users to track app engagement.

![KPI Distribution Matrix](./assets/KPI_3.png)
*(Fig 3: The internal distribution guide aligning data outputs with departmental actions.)*

---

## 🛠️ Concepts & Methodologies Applied
* **Data Modeling:** Star Schema Design, Fact & Dimension Table Structuring, Primary/Foreign Key Mapping.
* **Systems Architecture:** Software Dependency Mapping, Physical-to-Digital Data Capture (IoT, POS, API).
* **Business Intelligence:** Executive Dashboarding, Trend Analysis, ESG / B-Corp Reporting Integration.

---

## 👨‍💻 Authors & Acknowledgements
* **Vighnesh Shetty** - *Data Strategy & Architecture*
* **Mohit Bahukhandi** - *Data Strategy & Architecture*
* **Project Supervisor:** Prof. Antoine Jeanjean

---
*Too Good To Go exists to eliminate food waste globally. Every day, perfectly edible food is discarded — they're changing that, one rescued meal at a time.*
