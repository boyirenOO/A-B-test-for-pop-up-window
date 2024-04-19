# A-B-test-for-pop-up-window

## Washu Career Development Center: A/B Testing Course

### Introduction to A/B Testing at Washu
Washu's Career Development Center offers an insightful course on A/B Testing, also known as split tests. These are online experiments aimed at evaluating potential enhancements on the Career Development Center's course website. This course involves a walkthrough of a Python notebook focused on a real-world project, the "Study Plan" pop-up.

### Experiment Overview
**Experiment Name:** "Study Plan" Pop-up

**Conducted by:** Washu Career Development Center

**Business Goal:**
The main objective is to maximize the completion rate of our career development courses by students.

### Current Conditions Before the Change
Prior to the experiment, the homepage of our career development courses presented two main options:
- **Start Learning:** Upon selecting this option, students are introduced to the course content immediately.
- **Explore Courses:** This option allows students to browse course materials freely without enrollment.

### Description of the Experimented Change
In the experiment, a new "Study Plan" pop-up was introduced on the course homepage. When students chose to start learning, they were prompted to enter their available study hours per week:
- **5 or more hours:** Students proceed to access the course as usual.
- **Less than 5 hours:** A message suggested that successfully completing the course typically requires a greater time commitment, offering them the option to freely explore course materials instead.

### Experiment Hypothesis
The hypothesis was that by setting clearer expectations about the time commitment required upfront, the number of students who leave the course due to inadequate time would decrease, without significantly affecting the overall course completion rates. If proven true, this could enhance the student experience and allow better support from the center's staff for students more likely to complete the courses.

### Experiment Details
**Unit of Diversion:** Cookie-based, with further tracking by user-id once a student enrolls in any course.

### Metric Choice
**Invariate Metrics:** Clicks on "Start Learning" and "Explore Courses" - these should remain stable as they reflect basic engagement that should not be influenced by the experiment.
**Evaluation Metrics:** Conversion rate to active course participation and course completion rate. These metrics are directly impacted by the experiment and critical to the business goals. A significant change in these metrics, as defined by a minimum detectable effect (Dmin), would indicate the success or failure of the introduced changes.
