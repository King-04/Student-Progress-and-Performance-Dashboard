# Power BI Dashboard for Tracking Student Progress and Performance

## 📘 Project Overview

**Dare Careers** is a professional training organization that offers upskilling programs in **Power BI** and **AWS Cloud**.
To effectively monitor learner engagement, academic progress, and program outcomes, I developed a **Power BI dashboard** that tracks performance metrics such as attendance, participation, assessment scores, graduation, and certification rates.

This project demonstrates how data from multiple learning activities can be **transformed, modeled, and visualized** to generate actionable insights for educators and program managers.

---
![page 1](/dare1.png)

## 🎯 Objectives

The primary goal of this dashboard is to:

* Provide a **comprehensive view** of learner performance across different training tracks.
* Identify **trends and at-risk learners** through data-driven metrics.
* Enable **real-time monitoring** of participation, assessment, and certification outcomes.
* Support **decision-making** for improving program design and learner success.

---

## 🧩 Data Sources and Structure

The dataset was organized into multiple directories, each representing a key learning component for **two tracks** — *Power BI Training* and *Cloud Training*.

| Data Category             | Description                                     | Structure                           |
| ------------------------- | ----------------------------------------------- | ----------------------------------- |
| **Zoom Attendance**       | Daily attendance records per learner (10 weeks) | Week1–Week10 folders for each track |
| **Participation Records** | Daily engagement and participation scores       | Week1–Week10 folders                |
| **Lab and Quiz Grades**   | Weekly lab and quiz scores                      | Week1–Week10 folders                |
| **Status Records**        | Graduation and certification status             | One file per track                  |

Before importing into Power BI, the data was **cleaned and aggregated** in **Power Query** to ensure consistency across tracks and time periods.

---

## 🧠 Data Modeling and DAX

Data preparation and modeling involved:

* Establishing **relationships** between attendance, participation, assessment, and learner status tables.
* Using **DAX** to compute:

  * Attendance rate per learner
  * Average quiz and lab scores
  * Graduation and certification rates
  * Dropout and participation metrics
* Applying business logic (e.g., learners are marked “Attended” only if Zoom session duration > 30 minutes).

---

## 📊 Dashboard Overview

The dashboard consists of **two main report pages**:

![page 1](/dare1.png)
![page 2](/dare2.png)

### 1. **Overall Performance Metrics**

Provides a program-wide overview for stakeholders.

**Key Visuals:**

* **Bar Charts:**

  * Average assessment scores (labs and quizzes)
  * Average attendance and participation rates
  * Graduation, certification, and dropout rates by track
* **Summary Cards:**

  * Total Learners
  * Total Dropouts
  * Total Graduations
  * Total Certifications
* **Slicers (Filters):**

  * Learner Status, Track, Graduation Status, Certification Type

**Key Insights:**

* Overall learner base: **140**
* Total certifications: **92**
* Dropout rate: higher in Cloud Training (18%) compared to Power BI Training (14%)
* Certification rate: Power BI (68%), Cloud (60%)

---

### 2. **Learner Insights**

Drills down into individual learner performance for trainers and program managers.

**Key Visuals:**

* **Learner Table:**
  Displays each learner’s track, attendance rate, participation count, and average score.
* **Summary Cards:**

  * 1,400 Total Labs Completed
  * 10.57K Total Class Hours
  * 94.1% Average Attendance Rate
  * 50.81 Average Assessment Score
  * 6,037 Total Participation Count
* **Slicers:**

  * Track, Learner Status, Program Status, Month, Week

**Key Insights:**

* Power BI learners showed higher consistency in attendance and engagement.
* Assessment scores varied moderately across cohorts, suggesting areas for content improvement.

---

## 💡 Insights and Impact

This dashboard enables **data-driven monitoring** of training outcomes by:

* Highlighting **attendance and engagement patterns** across programs.
* Identifying learners **at risk of dropping out** early.
* Providing a **transparent overview** of certification and graduation trends.
* Supporting **strategic decisions** on training delivery and learner support.

---

## 🧰 Tools and Technologies

* **Microsoft Power BI** – Data modeling, visualization, and DAX
* **Excel / CSV** – Data preparation and cleaning
* **DAX** – Calculations for attendance, participation, certification, and performance metrics

---

> **Note:**
> This project was developed for portfolio and educational purposes using anonymized sample data.
