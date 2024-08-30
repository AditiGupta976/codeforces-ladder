# WolfOutLadder

## Overview
WolfOutLadder is a project aimed at helping Codeforces users improve their ratings by providing a curated selection of Codeforces questions. These questions are selected based on data from ideal candidates who have rapidly increased their ratings in specific brackets (1200-1400, 1400-1600, and 1600-1800). By analyzing the performance of these users, the platform offers a set of problems that are likely to help users advance in their competitive programming journey.

## Flowchart
![FlowChart](https://github.com/jot-s-bindra/C2Ladder/blob/master/WolfOut.drawio.png)

## Data Sources
- Data is primarily fetched from the Codeforces API.
- Users selected are those who crossed the given rating brackets in 4-5 contests or approximately 20-30 days, ensuring they are not old users and have no questions skipped in their contests. 

## Machine Learning Model
- The selection process involves data cleaning, feature scaling, and applying cosine similarity to identify questions that are most relevant to users within the targeted rating brackets.

## Feedback & Improvements
### Potential Enhancements:
1. **Diversity in Problem Selection**: Consider including a wider variety of problems by relaxing some of the strict filtering criteria. This could help cater to a broader audience.
2. **Regular Updates**: Implement a mechanism to regularly update the question pool as new contests and user data become available on Codeforces.
3. **Personalization**: Introduce user-specific recommendations based on individual progress and performance trends.
4. **Difficulty Calibration**: Ensure the difficulty level of the curated problems is consistent with the targeted rating bracket by cross-referencing with expert ratings or using additional machine learning models.

