# Advanced Analysis and Modeling
## Linear Regression Model: Title 42 vs 2019 Policy effects on repatriations counts
<img width="305" height="194" alt="image" src="https://github.com/user-attachments/assets/c2774d6f-06b6-475a-a15d-bccad5ada930" />
The linear regression model shows strong performance, with a low MAE and an R^2 of approximately 70.95%. This suggests that the model captures most of the variation in repatriation counts and is appropriate for interpreting policy effects and scenario 
analysis.

<img width="749" height="163" alt="image" src="https://github.com/user-attachments/assets/3f7f6920-4b1b-43a6-b6ac-cd5f2096fde4" />
<img width="743" height="253" alt="image" src="https://github.com/user-attachments/assets/bcbb8697-24e7-4a4d-b418-dd4298573348" />
The scenario results show that repatriation counts are consistently higher when Title 42 is active and lower when the 2019 enforcement regime is applied. Specifically, repatriations
increase from about 52,477 to 55,435 without the 2019 policy and from 47,865 to 50,563 when the 2019 policy is present. While these differences appear modest in absolute terms, this is largely due to the inclusion of lagged features, which anchor 
predictions to recent historical levels and dampen large fluctuations. As a result, policy effects operate as multiplicative adjustments on prior values rather than producing large independent jumps. This is supported by the model coefficients, where 
Title 42 corresponds to an approximate 5.6% increase in repatriation counts, while the 2019 enforcement regime is associated with a decrease of roughly 14–15%. Within this framework, the consistent increases observed under Title 42 scenarios indicate 
a positive and reinforcing effect on repatriation counts, whereas the 2019 enforcement regime is associated with reductions.

## Linear Regression Model: Pre vs During Title 42 Scenarios
<img width="603" height="102" alt="image" src="https://github.com/user-attachments/assets/607fe546-1414-487a-989e-0d4ec0cc8903" />
The regime model results show a clear increase in repatriation counts during the Title 42 period compared to before it. Specifically, predicted repatriations rise from about 64,871 in the pre Title 42 period to approximately 92,596 during Title 42, 
representing a substantial increase. While this model captures the overall structural shift between periods, it does not account for temporal dependencies. In contrast, the lag based model shows that changes in repatriation levels occur more gradually, 
with policy effects acting as multiplicative In [110… adjustments to prior values. Together, these results indicate that the spike observed during the Title 42 period reflects a sustained increase over time rather than a single period jump.

## XGBoost Model: Title 42 vs 2019 Policy effects on repatriations ratios
<img width="336" height="72" alt="image" src="https://github.com/user-attachments/assets/29884a23-82c7-4bb0-a317-34460381590b" />
The XGBoost model demonstrates strong predictive performance, with a low MAE of approximately 0.136 and an R^2 of about 0.85. This indicates that the model effectively captures variation in the repatriation-to-encounter ratio. Scenario analysis shows that 
the ratio remains largely stable across different policy combinations, with only a slight increase associated with the 2019 enforcement regime. Notably, the introduction of Title 42 does not significantly change the ratio, suggesting that enforcement 
efficiency remains relatively constant. These results indicate that increases in repatriation counts are not driven by improvements in efficiency, but rather by higher overall processing volume.
<img width="657" height="171" alt="image" src="https://github.com/user-attachments/assets/605537bd-175c-41ca-8feb-5bce135a7679" />
The ratio model results indicate that the repatriation to encounter ratio remains largely unchanged under Title 42, suggesting that increases in repatriation counts are not driven by improved efficiency. Instead, the stable ratio across scenarios implies 
that higher repatriation levels are primarily the result of increased processing volume rather than changes in perencounter outcomes.

## Conclusion
The results across all three models consistently indicate that Title 42 is associated with higher repatriation counts, while having little to no impact on the repatriation to encounter ratio. The policy scenario analysis shows that repatriations 
increase in all cases where Title 42 is active, regardless of the presence of the 2019 enforcement regime. Similarly, the regimebased model demonstrates a clear structural increase in repatriation levels during the Title 42 period, with predicted 
monthly counts rising notably compared to the pre–Title 42 period. In contrast, the ratio model shows that efficiency remains relatively stable across all scenarios, indicating that the proportion of encounters resulting in repatriation does not 
meaningfully change. Taken together, these findings suggest that the observed spike in repatriations is driven by increased processing volume under Title 42 rather than improvements in enforcement efficiency. While the lag-based model indicates that 
changes occur more gradually and are anchored to prior levels, policy effects operate as multiplicative adjustments that compound over time. In other words, Title 42 appears to enable enforcement at a larger scale rather than making the process more 
effective on a per-encounter basis. To further support and communicate these findings, the next phase of this analysis will focus on visualization in Tableau. Time series visualizations of repatriation counts will be used to clearly illustrate the spike
during the Title 42 period, while overlays or annotations will highlight when specific policies were active. Additional charts will compare repatriation counts and ratios across policy regimes, reinforcing the distinction between volume-driven
increases and stable efficiency. These visualizations will provide an intuitive, data-driven way to validate the modeling results and clearly demonstrate how Title 42 aligns with the observed increase in repatriations.
