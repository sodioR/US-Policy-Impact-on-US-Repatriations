# Data-Patterns-and-Representations-FP-BR-SR
## Final Project for Data Patterns and Representations conducted and curated by Sadia Rahman and Brooke Rice 

### Topic Selection: Impacts of Different Policy Regimes on U.S. Repatriation Metrics (2015–2025)
This topic will explore whether shifts in federal policy regimes are associated with structural changes in U.S. immigration enforcement outcomes between 2015 and 2025. Instead of focusing on a single policy, the analysis will build a custom policy regime dataset that captures broader enforcement environments, including administration transitions, national emergency declarations, public health emergency periods, and major enforcement mechanisms such as Title 42 and Title 8. The central research question guiding this topic is: <br>
***Are changes in repatriation and removal ratios associated with identifiable federal policy regime shifts over time?***
The goal is not to prove direct causation, but to evaluate whether enforcement outcome ratios show statistically meaningful shifts that align with broader regime changes. In other words, the analysis will assess whether measurable structural differences coincide with identifiable institutional transitions. <br>
This topic is socially relevant because immigration enforcement statistics are often discussed in public discourse using raw counts, without adjusting for overall encounter volume or considering broader structural context. By examining repatriation to encounter ratios across defined policy regimes, this topic moves beyond simple totals and instead looks at how enforcement intensity shifts over time. Focusing on structural changes rather than isolated numbers contributes to a more informed and data-driven discussion of immigration enforcement dynamics. <br>
Beyond identifying structural breaks, the analysis will explore whether regime effects appear immediately or with delay. Do repatriation rates shift at the same time as policy transitions, or do measurable changes occur after a lag? We aim that this topic will also examine whether ratio changes are primarily driven by fluctuations in encounter volume, changes in enforcement mechanisms, or shifts in demographic composition. <br>

### Dataset Identification: We aim to utilize three central datasets for this project.
- **[Department of Homeland Security (DHS) dataset for repatriations/removals:](<https://ohss.dhs.gov/khsm/dhs-repatriations#table-data-heading>)**
The DHS repatriations and removals dataset provides both annual and monthly counts of removals, returns, and repatriations. These measures represent downstream enforcement outcomes and will serve as the primary dependent variables.

- **[US Customs and Border Protection (CBP) dataset for encounters:](<https://www.cbp.gov/document/stats/nationwide-encounters>)**
This dataset provides totals across enforcement authorities, including Title 42 and Title 8, along with breakdowns by demographic category. Encounters represent inflow pressure and will be used as the denominator when constructing the repatriation to encounter ratio.

- **Custom Policy Regime Marker:**
The third dataset will be a custom created policy regime marker dataset. These markers will include administration period, public health emergency status, Title 42 activation period, national emergency status, and post policy termination phases. The aim is to overlay these markers with the repatriation to encounter ratios over time to answer our initial question on what the impact of these policies can look like.

Some additional questions we hope to answer: <br>
•	Does enforcement intensity become more variable during emergency periods compared to non-emergency periods? <br>
•	Are certain administrations associated with greater stability or volatility in repatriation rates? <br>
•	Do periods of rapid encounter growth correspond with declining repatriation ratios, potentially suggesting operational capacity constraints? <br>
•	Does the end of a policy regime lead to normalization, overshoot, or continued divergence in enforcement outcomes? <br>
•	Are observed ratio changes consistent across fiscal years, or concentrated within specific months? <br>
