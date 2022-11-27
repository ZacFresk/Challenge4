# PyCity School District Analysis

# Purpose

Maria had requested to review the top and bottom performing schools and their math and reading levels. She had also wanted to know the averages displaying each student. She then also wanted us to display the information and filter it by school size and type.

After the first review was sent in we were asked to complete another report for Thompson High School as the information they had submitted from their 9th grade class wasn't true as the students were dishonest. We were tasked with replacing all the data with NaNs to essentially remove the data so it wouldnt show up. After removing the data the code was reran to show the new values.

# Analysis Results

## How is the District Summary Affected?
- Original School Report

![Original_School_Summary_df](https://user-images.githubusercontent.com/107363203/204158845-16dc128b-e251-417b-845f-bbfb79af5412.png)

- Refactored School Report

![Refactored_District_Summary_df](https://user-images.githubusercontent.com/107363203/204158772-6b2e3788-a34b-48d1-aa8f-159a8339a03a.png)

**Impact of Removing the 9th Graders at Thompson High School**

After removing the false scores given by the 9th graders the district scores for math were lower with the reading scores having no change. The overall passing grade percentage was lower from 65.2% down to 64.9%.

## How is the School Summary Affected?
- Original School Report

![Original_School_Summary_df](https://user-images.githubusercontent.com/107363203/204158885-960fa97f-858b-4362-9e6b-5e80dc968714.png)

- Refactored School Report

Below is showing the district results using only the 10th to 12th grade scores at Thompson High School

![Refactored_School_Summary_df](https://user-images.githubusercontent.com/107363203/204158944-241a3fad-f4c5-4463-8f76-709a9b237cd9.png)

Below is showing the district results using all of 9th to 12th grade scores at Thompson High School, but the 9th grader's math and reading were NaN out. 

![Refactored_School_Summary_9to12_df](https://user-images.githubusercontent.com/107363203/204159006-4f5e2ca8-3684-4a67-86af-eb455ff6e0cb.png)

**Impact of Removing the 9th Graders at Thompson High School**

If we kept the data the 9th graders had given then the high school would suffer from the result. Thompson High School would suffer from lower test scores based on an entire 9th grade class getting 0's if we left the 9th graders in the review. Instead we only used the test data for the 10th to the 12th graders at Thompson High School. With the math scores dropping and reading staying having minimal change. More interesting was that the percent passing dropped for both reading and math and the overall passing dropped as well.

## How Does Replacing the 9th Graders’ Scores Affect Thompson High School's Performance Relative to the Other Schools?

- Original School Report

![Original_Top_Five_School](https://user-images.githubusercontent.com/107363203/204159022-3acd3413-e989-4e6d-8355-c175f4d59d6a.png)

- Refactored School Report

![Refactored_Top_Five_School](https://user-images.githubusercontent.com/107363203/204159029-14463cb5-cd3a-47b9-baeb-d4b5e76440bb.png)

**Impact of Removing the 9th Graders at Thompson High School**

With removing the false data from the 9th graders, Thompson High School would be considered second best when considering their overall passing percentage. Thompson High School would drop much lower in the rankings if the 9th graders scores were removed but the student count was not removed.

# How Does Replacing the 9th Grade Scores Affect the Following:

## Math and reading scores by grade

- The main difference here for the overall passing grades for individual grades was that the 9th grade scores were redacted. Overall, there was no significant change to the other scores. 

## Scores by school spending

![Scores_per_Spending_Bin](https://user-images.githubusercontent.com/107363203/204159037-54f025fc-c3b7-4fab-bd27-685de20dd8c9.png)

- The overall change for each schools spending range is nominal as, there isn't a noticeable change at the whole integer level. 

## Scores by school size

![Scores_by_school_size](https://user-images.githubusercontent.com/107363203/204159050-b79f7f6f-da79-487f-a5f7-1aebe465c20d.png)

- The change in passing rates are very little to the overall passing rates of the district if Thompson High School 9th grade scores are removed. 

## Scores by school type

![school_by_type](https://user-images.githubusercontent.com/107363203/204159053-242e7466-e1f1-43ac-bd44-68caa36335a7.png)

- The change here shows us that the change in overall passing scores of the district are very little when all the scores are combined. 

## Analysis Summary

When comparing the reading and math passing scores for Thompson High School. 
   - What are the schools passing score if the 9th grade scores are removed, but the student counts are kept in. 
   - What are the scores for only the 10th to 12th grades. 
   - If the 9th graders were kept in, Thompson High School' overall passing percentage dropped drastically from 90% to 65%. 
   - If the 10th to 12th graders are looked at alone, without the NaN scores the 9th grade scores and student count, then over passing scores change is very little.

When we review the overall placing of schools before and after the scores were removed. 
   - If the 9th grade student count is left in the school would drop to around mid-range in over all passing percentage. 
   - If only the 10 to 12th grade scores are reviewed, Thompson High School remains at second best overall scores. 

With the overall changes to the district reports, it would prompt for a more indepth report on the 9th grade students. If a review was conducted at this level it would show if there is a relevant difference between these schools. Thompson High School scores are comparable to other charter schools in the district or are they comparable to the capita budget category. A district level review shows the changes do not reflect a very large change. Conducting a different type of review may bring clearer information for the test scores at Thompson High School. 
