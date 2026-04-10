# MC_CapstoneProject


**Project Summary**

Master Control has two different products MX and QX. QX is a much more established product and has a higher conversion rate in the sales pipeline, compared to MX. QX converts at 19.7% vs 12.9% for MX. Data analysis was done to better predict what makes a good MX customer, so the sales pipeline could be more efficient. A pipeline was created to take leads and score them through a model to determine the probability they would progress through the sales pipeline.
Inbound sales leads over a two year period were analyzed. This contained information about the company that was interested in the product as well as information about how they came into the sales pipeline.
By creating this, Master Control can better utilize sales resources targeting and focusing on higher quality leads. The target audience for this was both the data analytics team and marketing, so both technical and business applications were considered and presented.


**Solution**

First, as a group, exploratory analysis to understand what factors were driving conversions was performed. This showed us that there was strong signal across various available data points, and missing or low quality data was a big predictor of leads not converting.
Next a data preprocessing pipeline was developed for cleaning and standardizing data. This would allow for future leads to easily be scored.
After this, several modeling approaches were attempted and then compared to determine which had the strongest predictive performance. One of the biggest concerns for this project was that any modeling performed was explainable, so black box models were not heavily explored. Regression, decision trees, random forest, XGBoost and EBM (explainable boosted model) were all utilized. Ultimately the EBM model was chosen as it had the best performance and was explainable.
Finally the model was applied to sample customer profiles to highlight the ideal customer profile and the effect it would have if applied.


**Business Value of Solution**

Estimated values were used for costs of outreach and the expected value of a won contract. An optimal probability threshold was then determined that equated with the highest expected value for the company. Given the low estimated cost of outreach ($1000) and high expected value of a won deal ($7.3 million), it was determined that any lead with a probability of greater than 10% of converting should be pursued. This allows the company to do two things; first determine what leads are worth pursuing in general and second prioritize by reaching out to the leads with the greatest likelihood of converting.


**My Contributions**

This project was completed with a group of four individuals. For my individual piece, I worked on the specialized data cleaning pipeline and analysis for one field, the job title of the contact who submitted for information. This was the only freeform field, and had huge variation which created unique problems for modeling. Of 16k sales leads about 6k had this field blank, of the populated 10k about 6k were unique. Several text preprocessing steps and tokenization were performed to keep these in for future modeling.
During the modeling steps, I focused on testing various iterations of regression models with various interactions, decision trees and XGBoost models.
For our final presentation I worked on explaining the job title analysis and cleaning, and other exploratory analysis.


**Difficulties Encountered**

Overall this analysis and project did go smoothly. The biggest problem we had was getting most of the various modeling approaches to give any meaningful performance. Given the exclusion of black box models, we were left with approaches that typically are underpowered due to their simplicity. In general, despite a lot of iterations and attempts, all of the various modeling approaches struggled to get close to the performance of EBM. Some models, like random forest, were prone to overfitting heavily which allowed them to get similar performance but then greatly underperformed on unseen data.


**Takeaways**

This project was a great opportunity to understand a real business problem, the stakeholders' needs, and come up with an actionable plan and insights. Having a specific business objective was a good opportunity to tailor the approach and kept the analysis and deliverables targeted and constrained. If modeling for just pure predictive power, the approaches taken would have been much more complicated, but having to work within given constraints to make it understandable was a good practice for real life future problems.
