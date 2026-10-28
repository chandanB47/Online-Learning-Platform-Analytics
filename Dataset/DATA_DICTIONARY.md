# Dataset Dictionary — Expanded Online Learning Platform Analytics

All data is synthetic and intended for Power BI practice. It does not describe a real company or real learners.

## Dataset scale
- Enrollments: 100,000 rows
- Learners: 10,000 rows
- Courses: 120 rows
- LearningActivity: 100,000 rows
- Instructors: 30 rows
- Enrollment date coverage: 2021–2025

## Table grain and relationships

| File | Grain | Key |
|---|---|---|
| `Enrollments.csv` | One row per learner-course enrollment | `EnrollmentID` |
| `Learners.csv` | One row per learner | `LearnerID` |
| `Courses.csv` | One row per course | `CourseID` |
| `LearningActivity.csv` | One summary row per enrollment | `ActivityID`; `EnrollmentID` links to enrollments |
| `Instructors.csv` | One row per instructor | `InstructorID` |

Suggested relationships:
- `Learners[LearnerID]` 1 → many `Enrollments[LearnerID]`
- `Courses[CourseID]` 1 → many `Enrollments[CourseID]`
- `Instructors[InstructorID]` 1 → many `Courses[InstructorID]`
- `Enrollments[EnrollmentID]` ↔ `LearningActivity[EnrollmentID]`: verify uniqueness on both sides; expected one-to-one
- Create a Date table and relate `Date[Date]` 1 → many `Enrollments[EnrollmentDate]`

Use single-direction filtering as the default. Do not merge LearningActivity into Enrollments in a way that duplicates enrollment-level revenue.

## Data-quality practice
The following issues are intentional:
- A few trailing spaces in `Enrollments[Device]`.
- Mixed capitalization in `Enrollments[AcquisitionChannel]`.
- Missing `DiscountPct` values.
- Blank `Learners[City]` values.
- A few blank/space-only `Courses[Category]` values.
- A small number of missing `LearningActivity[QuizAttempts]` values.

Inspect and document your treatment. Do not assume missing discount equals zero without a reason.

## Main fields
### Enrollments
IDs, enrollment/completion dates, status, list price, discount, amount paid, progress, rating, device, acquisition channel, payment method, coupon use, refund flag.

### Learners
Demographics, geography, signup date, learner type, employment status, education level, marketing source, preferred language.

### Courses
Category, difficulty, duration, list price, instructor, format, language, launch date, certificate availability, course status.

### LearningActivity
Lessons completed, minutes watched, last active date, quiz attempts, support tickets.

## Suggested business questions
1. How do enrollments and revenue trend by month/year?
2. Which categories and courses generate the most revenue?
3. Which acquisition channels have the strongest completion rate?
4. How do discount levels relate to amount paid and refunds?
5. Which learner segments enroll and complete most often?
6. What engagement patterns appear across completed, in-progress, and dropped enrollments?
7. Which course formats, difficulty levels, or languages perform well?
8. Do support tickets or quiz attempts differ by enrollment status?
9. Which instructors and courses have strong ratings?
10. How do performance patterns vary by region, device, and payment method?

## Caveat
Because the dataset is synthetic, patterns are for practicing analysis and must not be presented as actual business evidence.
