# 📊 Analysis of TED Talks Formats and Audience Engagement for Strategic Event Planning
## 📌 Business Case Overview
The client recently acquired a license to host official TED conferences and is currently in the planning stage of organizing their inaugural event. To ensure the launch captures the classic, memorable spirit of TED while maximizing audience engagement, the client requires a data-driven approach to select speakers, curate themes, and optimize event logistics. This analysis leverages historical data from 3,377 TED talks (1984–2021) to uncover the structural benchmarks of highly successful conferences.

## 🎯 Project Objectives
- Define the ideal event format: Identify typical conference characteristics, including optimal talk duration, speaker counts, and event frequency.

- Quantify Audience Engagement: Analyze behavior patterns across metrics such as views, applause volumes, and humor frequencies to pinpoint what resonates with viewers.

- Map Regional & Thematic Trends: Evaluate geographical distributions and popular topic tags to guide localized programming and content strategy.

## 🔗 Quick Links
* ▶ View Interactive Dashboard: Available via BI Platform (Top-Down Hierarchical Layout)

* 🛠 View SQL Extraction & Analytical Scripts: Hosted in the /src directory

## 🛠 Tech Stack
* **Database**: PostgreSQL (data-analyst-ted instance with events, speakers, and talks relational tables).

* **Data Processing**: SQL (DBeaver) — utilized for complex table joins (LEFT JOIN to retain empty conferences), text field filtering, aggregation, and Top-N ranking.

* **BI Platform**: Yandex DataLens — leveraged for building a top-down interactive dashboard equipped with global parameter filters and multi-field text search.

* ## 🔍 Research Approach
Data Integration & Scope Analysis: Consolidated 3,377 historical records spanning 1984–2021 across three relational tables using precise primary/foreign key connections to ensure comprehensive data integrity.

Top-Down Visualization Architecture: Structured the dashboard hierarchically, transitioning from high-level ecosystem metrics down to isolated conference aggregates, individual talk deep-dives, and granular row-level data.

Targeted SQL Query Segmentation: Designed custom SQL scripts to isolate high-performing segments, specifically extracting the Top 20 most frequent thematic tags and the Top 10 most acclaimed speakers based on aggregated audience reactions.

## 💡 Key Findings
Thematic Concentration: Audience interest heavily aggregates around specific topics, with a clear hierarchy established by the Top 20 most popular tags (e.g., specific domain clusters identified via text analysis).

Quantifiable Engagement Drivers: Memorable performances leave distinct footprints, showing strong correlations between the frequency of localized humor (Top 10 funniest talks) and massive global visibility (maximum view counts).

Speaker Profile Impact: Total audience appreciation—measured by cumulative applause counts—is strongly tied to the speaker's specific professional background (speaker_occupation), highlighting which industries command the most attention.

## 🚀 Strategic Recommendations
Optimize Event Scheduling: Structure the conference agenda around the historical baseline for audience retention by utilizing the calculated average talk duration (AVG(duration)) and keeping speaker volumes within proven comfort thresholds.

Curate High-Engagement Content: Anchor the event’s core themes within the identified Top 20 popular tags, and actively incorporate engaging, lighthearted, or humorous elements to replicate the classic TED atmosphere.

Target High-Impact Speaker Profiles: Prioritize recruiting speakers whose occupations and professional backgrounds align with the Top 10 profiles that historically generate the highest volumes of audience applause.

## 📁 Repository Structure
README.md — Project overview, technical specifications, and executive summary (this file).

/data — Anonymized sample dataset (dataset_clean.csv) limited to 1,000 entries to allow native browser rendering on GitHub.

/src — Production-ready SQL scripts detailing the data aggregation, cross-table joins, and ranking logic used for the dashboard charts.
