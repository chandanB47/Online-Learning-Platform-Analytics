# Online Learning Platform Analytics --- Power BI


**Status:** Initial dashboard release\
**Tools:** Power BI Desktop, Power Query, DAX\
**Dataset:** Synthetic online-learning platform data

## Project Overview

This project analyzes a synthetic online-learning platform using Power
BI. It demonstrates data cleaning, data modeling, DAX measures,
interactive visualizations, and business intelligence reporting.

The report explores enrollment trends, acquisition channels, learner
engagement, course performance, instructor performance, and data
quality.

## Dashboard Pages

### 1. Executive Overview

-   Total amount paid and total enrollments
-   Completion rate and average course rating
-   Completed enrollments and unique learners
-   Year slicer
-   Enrollment trend over time
-   Enrollment status distribution
-   Learner engagement versus progress

### 2. Enrollment & Acquisition Analysis

-   Amount paid by course category
-   Amount paid by acquisition channel
-   Enrollment volume by acquisition channel
-   Refund-flag rate by acquisition channel
-   Channel-level KPI comparison table
-   Category and payment method slicers

### 3. Learner Engagement

-   Total minutes watched
-   Total lessons completed
-   Average quiz attempts
-   Minutes watched by course and acquisition channel
-   Lessons completed by acquisition channel
-   Enrollment status distribution

### 4. Course Performance

-   Total courses and instructors
-   Average course rating
-   Top courses by amount paid
-   Amount paid by category and difficulty
-   Instructor comparisons by amount paid and rating

### 5. Data Quality & Definitions

-   Total and distinct enrollment ID checks
-   Duplicate enrollment ID checks
-   Missing course ID checks
-   Metric definitions and data limitations

## Business Questions

The report is designed to investigate: - How do enrollment volumes
change over time? - Which acquisition channels contribute the most
enrollments and amount paid? - Which course categories and courses have
the highest recorded amount paid? - How do completion and refund-flag
rates vary by acquisition channel? - How is learner engagement
associated with learning progress? - How do course and instructor
performance compare? - What data-quality limitations should be
considered before drawing conclusions?

## Tools & Techniques

-   **Power Query:** data preparation, type checking, text
    standardization, and data-quality checks
-   **Data modeling:** relationships between relevant tables and a date
    table
-   **DAX:** measures for enrollment volume, distinct learners, amount
    paid, completion rate, ratings, engagement, and refund-flag rate
-   **Power BI visuals:** KPI cards, line charts, bar and column charts,
    a doughnut chart, a scatter plot, slicers, and a comparison table

## Data & Interpretation Notes

-   The dataset is synthetic and does not represent an actual learning
    platform.
-   `Amount Paid` is not necessarily net revenue.
-   A refund flag does not independently establish that a cash refund
    occurred.
-   Engagement and progress associations do not establish causation.
-   Results should be interpreted in the context of report filters,
    metric definitions, and data quality.
-   Validate reported figures against the source data and data model
    before using them for business decisions.

## Repository Contents

The repository currently includes project documentation and a `Dataset/`
folder. Before publishing Version 1.0, include the final Power BI report
(`.pbix`), relevant source datasets, and report screenshots where
appropriate.

Suggested structure:

``` text
Online-Learning-Platform-Analytics/
├── Dataset/
├── Screenshots/
├── Online-Learning-Platform-Analytics.pbix
└── README.md
```

Adjust the structure above to match the actual files committed to the
repository. Do not include private, confidential, or licensed data
without permission.

## How to View the Report

1.  Download the `.pbix` file from this repository once it has been
    uploaded.
2.  Open it in Power BI Desktop.
3.  If prompted, point the queries to the included source data files and
    refresh the data.
4.  Navigate through the five report pages and interact with the
    slicers.

## Project Status

The five report pages have been built in Power BI Desktop. Before
calling this a complete Version 1.0 release, verify that the `.pbix`
file and intended source assets are committed to GitHub and that key
totals and slicers have been tested.

## Author

**Chandan B**\
GitHub: https://github.com/chandanB47
