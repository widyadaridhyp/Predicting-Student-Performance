# Predicting-Student-Performance

**Problem:**
Students exhibit significant variation in academic performance influenced by study habits, parental support, tutoring, and extracurricular participation. A lack of understanding of the key factors driving these outcomes makes it difficult for schools to provide targeted interventions and support at-risk students.

**Goals:**
1. Predict students’ Grade Class based on demographic details, study habits, parental involvement, and extracurricular activities.
2. Identify the most influential factors affecting academic achievement.
3. Provide actionable recommendations for effective educational interventions to improve student outcomes.

**Dataset:**
StudentID: A unique identifier assigned to each student (1001 to 3392).
> Demographic Details
- Age: The age of the students ranges from 15 to 18 years.
- Gender: Gender of the students, where 0 represents Male and 1 represents Female.
- Ethnicity: The ethnicity of the students, coded as follows:
  - 0: Caucasian
  - 1: African American
  - 2: Asian
  - 3: Other
- ParentalEducation: The education level of the parents, coded as follows:
  - 0: None
  - 1: High School
  - 2: Some College
  - 3: Bachelor's
  - 4: Higher
> Study Habits
- StudyTimeWeekly: Weekly study time in hours, ranging from 0 to 20.
- Absences: Number of absences during the school year, ranging from 0 to 30.
- Tutoring: Tutoring status, where 0 indicates No and 1 indicates Yes.
> Parental Involvement
- ParentalSupport: The level of parental support, coded as follows:
  - 0: None
  - 1: Low
  - 2: Moderate
  - 3: High
  - 4: Very High
> Extracurricular Activities
- Extracurricular: Participation in extracurricular activities, where 0 indicates No and 1 indicates Yes.
- Sports: Participation in sports, where 0 indicates No and 1 indicates Yes.
- Music: Participation in music activities, where 0 indicates No and 1 indicates Yes.
- Volunteering: Participation in volunteering, where 0 indicates No and 1 indicates Yes.
> Academic Performance
- GPA: Grade Point Average on a scale from 2.0 to 4.0, influenced by study habits, parental involvement, and extracurricular activities.
> Target Variable: Grade Class
- GradeClass: Classification of students' grades based on GPA:
  - 0: 'A' (GPA >= 3.5)
  - 1: 'B' (3.0 <= GPA < 3.5)
  - 2: 'C' (2.5 <= GPA < 3.0)
  - 3: 'D' (2.0 <= GPA < 2.5)
  - 4: 'F' (GPA < 2.0)
 
**Insight and Recommendation:**
- For students:
  - Take advantage of tutoring if there is material that you do not understand.
  - Increase extracurricular and music activities to maintain mental balance and focus on learning.
  - Keep absences to a minimum so you don't miss any material.
  - Add weekly study time to reinforce your understanding of the material.
- For schools:
  - Utilize tutoring if there is material that is not understood.
  - Increase extracurricular and music activities to maintain mental balance and focus on learning.
  - Keep absences to a minimum so as not to miss material.
  - Add weekly study time to reinforce understanding of the material.
- For prediction models:
  - Want high accuracy → Gradient Boosting
  - Want a more stable model with better generalization → Ada Boost
