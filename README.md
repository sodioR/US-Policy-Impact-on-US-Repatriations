# Impacts of Different Policy Regimes on U.S. Repatriation Metrics (2015–2025)
## Final Project for Data Patterns and Representations conducted and curated by Sadia Rahman and Brooke Rice 

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

The initial question asked whether changes in repatriation ratios are associated with identifiable federal policy regime shifts. After examining the visuals and summary statistics, it is clear that the ratio does not remain stable over time. Instead, it shows noticeable structural movement beginning around FY2020, which suggests that something broader than random fluctuation may be occurring. <br>
The ratio line plot, boxplot by administration, and scatter plot together show that enforcement intensity is not constant and does not scale proportionally with encounter volume. As encounters increase sharply, the share resulting in repatriation declines. This suggests that enforcement output may be influenced by institutional conditions rather than simply by inflow pressure alone. <br>

Based on these findings, the research focus shifts slightly. Instead of only asking whether regime shifts are associated with changes in the ratio, the analysis now considers more specific questions: <br>
-	Does enforcement intensity decline during high volume encounter periods? <br>
-	Do legal regime shifts, such as the implementation of Title 42, alter the relationship between encounters and removals? <br>
-	Are observable structural breaks in the ratio aligned with administration transitions? <br>
-	Does enforcement variability increase during emergency or public health periods? <br>

The EDA results suggest that enforcement dynamics are sensitive to regime context. Rather than comparing raw counts alone, the next stage of analysis should focus on structural classification of policy periods and testing for regime aligned shifts in enforcement intensity. This approach remains consistent with the project’s objective of identifying structural differences across enforcement environments

## EDA Overview

### Construction of Enforcement Intensity Ratio and Basic Statistics:
To move beyond raw totals, annual encounter totals were aggregated and merged with annual DHS repatriations to construct a “repatriation to encounter” ratio:

$$Ratio = Repatriations/Encounters$$

This ratio represents enforcement intensity (the share of encounters that result in repatriation).

## Summary Statistics for the Ratio

<img width="542" height="152" alt="Ratio representing enforcement intensity " src="https://github.com/user-attachments/assets/0e6bf4da-e48d-4b1d-836d-e17af9746ea8" /> <br>

The relatively large standard deviation indicates meaningful variability across fiscal years. Most notably, the ratio declines steadily even as raw encounter volume increases dramatically.
This confirms that enforcement output does not scale proportionally with inflow pressure. <br>

-	**Ratio by Fiscal Year Line Plot: The line plot demonstrates structural decline:** <br>

<img width="929" height="497" alt="Ratio FY chart" src="https://github.com/user-attachments/assets/3d3aff22-2d12-4597-881d-78e4f3e6942c" /> <br>

-	**Histogram of Ratio: The histogram shows distributional shift over time:** <br>

<img width="652" height="406" alt="ratio histogram" src="https://github.com/user-attachments/assets/63f4bd8b-362b-4b4a-9eeb-7eb591c407ca" /> <br>

### Scaling Behavior and Capacity Constraints

To better understand how encounter volume relates to enforcement outcomes, a scatter plot comparing Encounters and Repatriations was created. This visualization helps show whether removals increase at the same rate as inflow pressure or if the relationship changes as encounters rise. <br>
The scatter plot shows that repatriations do generally increase as encounters increase, but the relationship is not proportional. At lower encounter levels, repatriations appear more tightly clustered. However, as encounters reach higher levels, the spread in repatriation totals becomes much wider. This means enforcement output becomes less predictable during peak inflow periods. In other words, the system does not seem to operate at a constant processing rate. Instead of scaling evenly with encounter growth, repatriations fluctuate more as pressure increases. <br>
This pattern suggests that enforcement intensity may decline during periods of rapid encounter growth. When encounters surge, the share that results in repatriation appears to fall, which could reflect operational capacity limits, legal constraints, or broader institutional shifts. Rather than simply reflecting higher volume, the relationship between encounters and removals seems sensitive to structural conditions. <br>
This directly connects to one of the additional research questions outlined in the project proposal, which is whether periods of rapid encounter growth correspond with declining repatriation ratios, potentially indicating operational capacity constraints  <br>
The scatter plot provides early exploratory evidence that such a relationship may exist and warrants further structural analysis. <br>

-	**Scatter Plot: Encounters vs Repatriations:** <br>

<img width="688" height="474" alt="Encounters v Repatriations" src="https://github.com/user-attachments/assets/f400d15b-c36b-4ff3-9d0d-8c03ed69bc44" /> <br>
