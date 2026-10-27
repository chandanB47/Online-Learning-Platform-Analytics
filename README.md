# Online Learning Platform Analytics — Power BI

**Status:** In progress  
**Tools:** Power BI Desktop, Power Query, DAX  
**Data:** Synthetic online-learning dataset (to be added with the completed project)

## Project overview

This portfolio project will use Power BI to analyze an online learning platform. The goal is to create an interactive report that explores enrollment trends, course and instructor performance, learner engagement, completion outcomes, and acquisition channels.

The project will use Power BI only:
- **Power Query** for data preparation and quality checks
- **Power BI data model** for table relationships
- **DAX** for measures and KPIs
- **Power BI visuals** for interactive reporting

## Planned report pages

1. **Executive Overview** — enrollment volume, unique learners, amount paid, completion rate, refund-flag rate, and trends.
2. **Enrollment & Acquisition** — acquisition channels, enrollment status, devices, payment methods, and changes over time.
3. **Course & Instructor Performance** — course and category comparisons, ratings, and instructor performance.
4. **Learner Engagement** — learning minutes, lessons completed, quiz attempts, progress, and support tickets.
5. **Data Quality & Definitions** — data-quality checks, metric definitions, and known limitations.

## Business questions

The completed report will investigate questions such as:

- How have enrollments changed over time?
- Which acquisition channels contribute the most enrollments?
- Which courses have high enrollment volume and high completion rates?
- How do completion and refund-flag rates vary across channels and categories?
- How does learner engagement vary by enrollment status?
- Which instructors and courses perform well when enrollment volume is considered?
- What data-quality issues could affect the conclusions?

These are questions to investigate, not findings. Results will be added only after they have been calculated and validated in Power BI.

## Planned repository contents

As the project progresses, this repository will be updated with:

- Source datasets and a data dictionary
- Power Query cleaning notes
- Data model and relationship documentation
- DAX measures and metric definitions
- Business and analytical questions
- Screenshots of the completed report
- The finished Power BI report file, subject to repository size limits

**Note:** This initial repository contains project scope and plans only. The datasets, report file, and supporting project assets will be uploaded after the analysis and dashboard are completed.

## Data and interpretation notes

- The dataset is intended to be synthetic; findings will not be presented as claims about a real company or real learners.
- `Amount Paid` will not be described as net revenue unless refund treatment is verified.
- A refund flag will not be treated as proof that cash was refunded.
- Missing values will be investigated rather than automatically replaced with zero.
- Business conclusions will include the relevant denominator, filter context, and limitations.

## Project status

- [ ] Import and inspect source data in Power Query
- [ ] Clean data and document decisions
- [ ] Create and validate the data model
- [ ] Create and test DAX measures
- [ ] Build report pages
- [ ] Validate totals and slicers
- [ ] Record evidence-backed insights
- [ ] Add screenshots and final project files

## About

This repository documents a Power BI portfolio project focused on practical business intelligence, data modeling, and analytical reporting.
