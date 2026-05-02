# Exploratory Data Analysis (EDA):
## Project Context
This project examines whether shifts in federal policy regimes are associated with structural changes in U.S. immigration enforcement outcomes between 2015 and 2025. Rather than focusing on raw totals, the analysis centers on the “repatriation to encounter” ratio as a measure of enforcement intensity. The goal is not to prove causation, but to evaluate whether observable structural differences in enforcement outcomes coincide with identifiable regime transitions such as administration changes and Title 42 activation.

##Numerical and Categorical Features 
The DHS repatriations dataset mainly includes annual removal totals by fiscal year, along with several categorical breakdowns such as repatriation type, criminal vs non criminal status, arrest location, citizenship, and agency. For this EDA, the most important numerical variable is the annual repatriation total (quantity), since it represents the outcome side of immigration enforcement. These values are count based, meaning they are whole numbers and cannot be negative, and they show noticeable variation across fiscal years. This variability becomes clear in the Annual Repatriations line plot shown below, where we can see fluctuations over time rather than a stable pattern.
The CBP encounters dataset, on the other hand, represents inflow pressure. Its main numerical variable is Encounter Count, which captures how many individuals were encountered in a given fiscal year. In addition to year level totals, this dataset includes several categorical dimensions such as Land Border Region, Area of Responsibility, State, Demographic category, Citizenship, Title of Authority, and Encounter Type. These categories help describe not just how many encounters occurred, but also under what legal authority and in which geographic or demographic context they occurred. The Annual Encounters line plot below shows a sharp increase beginning around FY2020, highlighting how dramatically inflow pressure changes during this period.
Comparing the two visuals side by side reveals an important pattern. While encounters increase sharply after FY2020, repatriations do not rise at the same rate and eventually decline. This suggests that enforcement outcomes may not scale proportionally with encounter volume. Additionally, the categorical breakdown in the encounters dataset shows a clear distinction between Title 42 and Title 8 authority, which is important given the project’s focus on policy regimes. The Encounters by Title of Authority visualization further supports this by showing how legal authority shifts during peak encounter years, reinforcing the broader regime based framing described in the project proposal.


- ***Annual Encounters Line Plot*** <br>
 <img width="589" height="470" alt="Annual Encounters Line Plot" src="https://github.com/user-attachments/assets/fde0c687-bbb7-4046-88fb-1306d4c0f71e" /> <br>


- ***Annual Repatriations Line Plot*** <br>
<img width="616" height="463" alt="Annual Repatriations Line Plot" src="https://github.com/user-attachments/assets/7400d1d7-e4f0-4d4e-a79d-14c7a7867172" /> <br>


These establish the raw structure of the numerator and denominator.

## Construction of Enforcement Intensity Ratio and Basic Statistics 
To move beyond raw totals, annual encounter totals were aggregated and merged with annual DHS repatriations to construct a “repatriation to encounter” ratio:

$$
\text{Ratio} = \frac{\text{Repatriations}}{\text{Encounters}}
$$

This ratio represents enforcement intensity (the share of encounters that result in repatriation).

**Summary Statistics for the Ratio** <br> <br>
<img width="542" height="152" alt="Ratio representing enforcement intensity " src="https://github.com/user-attachments/assets/cb956967-d25b-4ca5-8f56-58dcdb0fbb77" /> <br>

The relatively large standard deviation indicates meaningful variability across fiscal years. Most notably, the ratio declines steadily even as raw encounter volume increases dramatically.
This confirms that enforcement output does not scale proportionally with inflow pressure.


- ***Ratio by Fiscal Year Line Plot: The line plot demonstrates structural decline.*** <br>
<img width="929" height="497" alt="Ratio FY chart" src="https://github.com/user-attachments/assets/29b709ed-5555-4f79-b15d-9eb0d959e65f" /> <br>


- ***Histogram of Ratio: The histogram shows distributional shift over time.*** <br>
<img width="652" height="406" alt="ratio histogram" src="https://github.com/user-attachments/assets/6bd385d5-3e79-4cb9-abab-75340dd3c6c9" /> <br>


## Structural Patterns and Regime Differences
The Ratio by Fiscal Year line plot shows a clear downward trend starting around FY2020. Even though repatriations increase at first, they do not keep up with the rapid growth in encounters. As encounters surge, the ratio steadily declines, meaning a smaller share of encounters results in repatriation over time. This creates a noticeable gap between inflow pressure (encounters) and enforcement output (repatriations). The visual makes this pattern much easier to see than looking at raw numbers alone.
To explore whether these changes might be connected to broader institutional shifts, a boxplot of the ratio by administration was created. The boxplot shows that enforcement intensity is not evenly distributed across administrations. Instead, the ratio varies in level and spread depending on the time period. This suggests that enforcement outcomes may be influenced by broader regime conditions, not just by how many people are encountered at the border.
The Encounters by Title of Authority visualization adds another layer to this analysis. It shows how the use of Title 42 and Title 8 changes over time, especially during peak encounter years. Since Title 42 represents a major legal mechanism during the public health emergency period, shifts in authority likely affect how encounters are processed. Seeing these authority changes alongside the declining ratio provides additional context for why enforcement intensity may be shifting.
Overall, these visuals support the project’s main objective, where instead of focusing only on raw totals, the analysis looks for structural differences in enforcement intensity that align with broader policy regimes. The patterns in the ratio line plot, administration boxplot, and authority breakdown together suggest that enforcement dynamics change across institutional environments rather than remaining constant over time.


- ***Boxplot of Ratio by Administration*** <br>
 <img width="906" height="508" alt="Boxplot of Ratio by Administration" src="https://github.com/user-attachments/assets/950fbb3b-7830-425f-8b1d-05196c19f65d" /> <br>


- ***Encounters by Title of Authority*** <br>
 <img width="632" height="214" alt="Encounters by Title of Authority" src="https://github.com/user-attachments/assets/a24b7c9d-c69f-4017-9095-c9e12b7c5cf3" /> <br>


## Scaling Behavior and Capacity Constraints
To better understand how encounter volume relates to enforcement outcomes, a scatter plot comparing Encounters and Repatriations was created. This visualization helps show whether removals increase at the same rate as inflow pressure or if the relationship changes as encounters rise.
The scatter plot shows that repatriations do generally increase as encounters increase, but the relationship is not proportional. At lower encounter levels, repatriations appear more tightly clustered. However, as encounters reach higher levels, the spread in repatriation totals becomes much wider. This means enforcement output becomes less predictable during peak inflow periods. In other words, the system does not seem to operate at a constant processing rate. Instead of scaling evenly with encounter growth, repatriations fluctuate more as pressure increases.
This pattern suggests that enforcement intensity may decline during periods of rapid encounter growth. When encounters surge, the share that results in repatriation appears to fall, which could reflect operational capacity limits, legal constraints, or broader institutional shifts. Rather than simply reflecting higher volume, the relationship between encounters and removals seems sensitive to structural conditions.
This directly connects to one of the additional research questions outlined in the project proposal, which is whether periods of rapid encounter growth correspond with declining repatriation ratios, potentially indicating operational capacity constraints. The scatter plot provides early exploratory evidence that such a relationship may exist and warrants further structural analysis.


- ***Scatter Plot: Encounters vs Repatriations*** <br>
 <img width="688" height="474" alt="Encounters v Repatriations" src="https://github.com/user-attachments/assets/9b56af78-141c-42d7-8a4b-aad264f3c1c2" /> <br>


## Refinement of Research Questions
The initial question asked whether changes in repatriation ratios are associated with identifiable federal policy regime shifts. After examining the visuals and summary statistics, it is clear that the ratio does not remain stable over time. Instead, it shows noticeable structural movement beginning around FY2020, which suggests that something broader than random fluctuation may be occurring.
The ratio line plot, boxplot by administration, and scatter plot together show that enforcement intensity is not constant and does not scale proportionally with encounter volume. As encounters increase sharply, the share resulting in repatriation declines. This suggests that enforcement output may be influenced by institutional conditions rather than simply by inflow pressure alone.
Based on these findings, the research focus shifts slightly. Instead of only asking whether regime shifts are associated with changes in the ratio, the analysis now considers more specific questions: <br>
- Does enforcement intensity decline during high volume encounter periods? 
- Do legal regime shifts, such as the implementation of Title 42, alter the relationship between encounters and removals? 
- Are observable structural breaks in the ratio aligned with administration transitions? 
- Does enforcement variability increase during emergency or public health periods?
The EDA results suggest that enforcement dynamics are sensitive to regime context. Rather than comparing raw counts alone, the next stage of analysis should focus on structural classification of policy periods and testing for regime aligned shifts in enforcement intensity. This approach remains consistent with the project’s objective of identifying structural differences across enforcement environments


