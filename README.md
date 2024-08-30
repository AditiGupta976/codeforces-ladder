# WolfOutLadder

## Overview
WolfOutLadder is designed to help Codeforces users improve their ratings by offering a carefully curated selection of problems. These problems are chosen based on the historical data of "ideal candidates," who have successfully navigated specific rating brackets (1200-1400, 1400-1600, 1600-1800) within a short period. By studying the problem-solving patterns of these candidates, WolfOutLadder aims to provide a targeted problem set that can help users effectively advance their competitive programming skills.

## Flowchart
![FlowChart](https://github.com/jot-s-bindra/C2Ladder/blob/master/WolfOut.drawio.png)

## Data Flow
- **Data Collection**: The platform pulls data directly from the Codeforces API, focusing on users who have demonstrated rapid rating improvement. The criteria for selection include:
  - Users who advanced through the rating bracket in 4-5 contests or within 20-30 days.
  - Users who are not long-time participants on the platform.
  - Users who did not skip questions and maintained consistent participation during this period.
  
- **Flask Server**: This data is sent to our Flask server, where it is processed and cleaned. The server also handles API requests from the frontend, ensuring that the data is presented in an accessible and user-friendly manner.

- **Frontend Integration**: The frontend uses the Flask server's API to dynamically map the processed data, generating personalized links to Codeforces problems. This ensures that users are always presented with relevant and up-to-date problem sets.

## Machine Learning Model
- **Feature Engineering**: The data undergoes a process of cleaning and feature scaling to ensure consistency and accuracy.
- **Cosine Similarity**: We apply cosine similarity to match users with problems that closely align with those solved by our ideal candidates. This approach helps in identifying problems that are likely to aid in rating improvement.

## Feedback & Improvements
### Potential Enhancements:
1. **Diversity in Problem Selection**: By relaxing some filtering criteria, we can include a wider variety of problems, which could appeal to users at different skill levels.
2. **Regular Updates**: Implement a system to automatically update the problem set as new contests are held and more data becomes available on Codeforces.
3. **Personalization**: Develop algorithms to provide personalized problem recommendations based on each user's individual progress and performance trends.
4. **Difficulty Calibration**: Regularly review the difficulty levels of selected problems to ensure they are consistent with the target rating brackets. This could involve cross-referencing with expert ratings or incorporating additional machine learning models.

## Future Scope
- **User Profiles**: Develop detailed user profiles where individuals can track their problem-solving progress, receive personalized recommendations, and set goals for their competitive programming journey.
- **AI-Powered Insights**: Leverage advanced AI techniques to provide deeper insights into a user's strengths and weaknesses, offering tailored practice suggestions.
- **Mobile App Development**: Extend the platform to mobile devices, enabling users to practice on-the-go and improving accessibility.
- **Community Features**: Introduce features like global leaderboards, discussion forums, and peer-to-peer challenges to create a more engaging and interactive user experience.


## Website
Explore the platform: [CodeLadderForces](https://codeladderforces.netlify.app)
