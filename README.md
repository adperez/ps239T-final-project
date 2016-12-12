Amanda D. Perez PS239T Final Project
## Short Description

This project's main goal was to look at data produced from the
greater good science center's online science of happiness class. 
The scripts do extensive cleaning of the data (specifically-the Qualtrics data).
Quantitative analyses were done and consisted of various linear regressions and correlations. These analyses were able to see which components of the course contributed the most to course performance and student happiness. 
Qualitative analyses were done and consisted of pre-processing, looking at word frequencies, sentiment analyses, and word clouds. These text analyses showed what students liked the most about the course in addition to areas for impovement.
GGplot2 & corrplot were used to produce all of the graphs. 

*Note* I removed all personally identifiable information from the datasets. Namely,I removed "edX_ID" & "User_ID". While they are referenced throughout the scripts, they are not included in the datasets. This was a necessary step in order for me to be able to share the rest of the data. 

## Dependency

1. R, version 3.3.1

## Files:

### Data

1. post_course_survey.csv:  Qualtrics survey data given to students of the
science of happiness after the course ended. 
2. edx_data.csv: Data produced on the course platform edX.org (e.g. exam scores). 
3. Dataset_For_Quantitative_Analysis.csv: The final Analysis Dataset derived from the raw data above. It includes nearly 200 variables, but below are a few (but not all) of most interest:
    - *Final*: Final exam score
    - *SHS*: Subjective Happiness
    - *STRESS*: Stress
    - *LONELY*: Loneliness
    - *Weekly_Hours*: Hours per week spent on the course
    - *Enrollment.Track*: Which track students were on, either verfified (paid) or audit(free).

### Code

1. 01__merge-data.Rmd: Loads, cleans, and merges the raw datasets (pre-course & edx).
2. 02_quantitative-analysis.Rmd: Conducts qualitative analyses of the data. Specifically, linear regressions and correlations are run.
3. 03_pre-processing-text.Rmd: Conducts pre-processing of text data, specifically this looks at what students liked the most & what suggestions for improving the course they have.
4. 04_sentiment-analysis.Rmd: Calculates the polarity of text statements of how the course impacted the students.
5. 05_visualizations.Rmd: Creates all of the graphs to accompany the qualitative & quantitative analyses.

### Results

1. Correlation_Matrix.pdf: Graphs the correlation matrix of Happiness, sense of purpose, loneliness, and stress.
2. frequency_liked_most.pdf: Shows the most frequent words that came up in the open ended responses of what was liked the most about the course.
3. frequency_suggestions.pdf: Shows the most frequent words that came up in the open ended responses of what could be improved about the course.
4. hours_spent_course_impact.pdf: Graphs the polarity of the open ended text response of how the course impacted the students. It is seperated by weekly hours spent on course.
5. ideal_self_happiness.pdf: Shows that higher frequency of partaking in the ideal self happiness practice leads to higher subjective happiness. Linear regression line is fitted.
6. mindful_breathing_exams.pdf: Shows that higher frequency of partaking in the mindful breathing happiness practice leads to higher final exam scores. Linear regression line is fitted.
7. random_kindness_happiness.pdf: Shows that higher prequency of partaking in random acts of kindness leads to higher subjective happiness. Linear regression line is fitted.
8. stress_exams.pdf: Shows that higher stress leads to lower exam scores. Linear regression line is fitted.
9. time_exams.pdf: Shows that the more time spent each week on the class, the higher the exam grades are. Linear regression line is fitted.
10. verified_track_course_impact.pdf: Graphs the polarity of the open ended text response of how the course impacted the students. It is seperated by enrollment track (verified vs audit).
11. cerified_track_exams.pdf: Shows that those who paid for a verified certificate do better on the final exam.
12. word_cloud_liked_most.pdf: Word cloud of most frequent words in the open ended response of what the students like the most about the course.
13. word_cloud_suggestions.pdf: Word cloud of the most frequent words in the open ended response of what could be improved about the course.

## Contact Information

Amanda D. Perez, Graduate student of Psychology. Contact: adpc@berkeley.edu
