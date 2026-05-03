# Policy Impact on US Repatriations
**Authored by** Sadia Rahman and Brooke Rice

## Topic Ovevrview
- We aimed to examine how U.S. immigration policy shifts affected border enforcement outcomes, primarily from 2015 to 2025. 
- We compared Title 8 Addendum policies such as MPP((Migrant Protection Protocol) with the later Title 42 framework to determine what drove spikes in reported encounters and repatriations. 
- Using monthly DHS (Department of Homeland Security), CBP (Custom and Border Protection), and a custom policy timeline data, the analysis tests whether increases reflected stronger traditional enforcement or a shift to faster expulsion mechanisms. 

## Policy Markers Included in Analysis
<img width="969" height="887" alt="image" src="https://github.com/user-attachments/assets/66b2e27b-8544-4c06-813c-da8dd7061842" />

## Annual Repatriation Types and Trends
<img width="1322" height="900" alt="image" src="https://github.com/user-attachments/assets/1faedfb1-ac36-4d91-bdb7-0919608964c1" />
Approximately 74% of all repatriations recorded during the Title 42 period were classified as Title 42 expulsions. This shows that the sharp increase in total repatriation activity from 2020 through 2023 was driven predominantly by the introduction of a new rapid-expulsion processing mechanism rather than a broad expansion of traditional enforcement categories such as removals, administrative returns, or enforcement returns. In other words, the surge reflected a shift in how repatriations were processed and counted, not simply stronger performance under pre-existing Title 8 enforcement systems.

## Monthly Repatriations vs Encounters
<img width="1033" height="1103" alt="image" src="https://github.com/user-attachments/assets/889f4adc-be62-455d-afc0-9f85a8559fb4" />
During the Title 42 period, encounters rose at a much faster pace than repatriations, producing the largest sustained gap between incoming border activity and enforcement outcomes from 2021 through 2023. While repatriations also increased and reached historic highs, they did not expand proportionally to the surge in encounters. This suggests that Title 42 coincided with significantly higher processing volume and system pressure, but not a matching increase in enforcement throughput relative to demand.

## Efficiency Ratio
$$
\text{Ratio} = \frac{\text{Repatriations}}{\text{Encounters}}
$$

<img width="1124" height="765" alt="image" src="https://github.com/user-attachments/assets/2c6aa02f-d431-4468-8b2b-76cd13fb8ba2" /> <br>

**Ratio Definition:** <br>
The efficiency ratio is calculated as Repatriations divided by Encounters. It measures how many repatriation outcomes occurred for each recorded encounter during a given year. <br>
**What It Represents:** <br>
A higher ratio suggests repatriation outcomes were keeping pace with, or exceeding, encounter volume. A lower ratio suggests encounters were growing faster than repatriation outcomes, indicating greater system pressure or reduced conversion of encounters into repatriations. <br>
**Interpretation:** <br>
The ratio declines substantially over the study period, falling from 1.34 in 2009 to 0.31 in 2024. Although temporary increases appear during the early Title 42 period, the long-run trend suggests that encounters ultimately expanded faster than repatriation outcomes. This indicates higher enforcement volume, but no sustained improvement in operational efficiency. 

## Model Overview
<img width="1065" height="460" alt="image" src="https://github.com/user-attachments/assets/9a4b73fc-5ee4-47f3-8a3c-54cae6823051" />
The count model used a logged repatriation outcome, so the coefficients appear small initially. After converting them back to the original count scale using e^coefficient, they represent meaningful percentage changes in predicted repatriation totals.

The clearest positive effect appears in the Title 42-only scenario, where a coefficient of 0.0548 converts to a 1.056× multiplier, or an estimated 5.6% increase in predicted repatriation counts. In contrast, the MPP / 2019 enforcement regime-only scenario has a coefficient of -0.0920, which converts to a 0.912× multiplier, or an estimated 8.8% decrease in predicted counts.

While the scenario ratio model predicted only modest differences across policy combinations, the observed historical repatriation-to-encounter ratio trends downward over time. This suggests Title 42 increased total enforcement volume, but did not generate a sustained improvement in operational efficiency, as encounters ultimately rose faster than repatriation outcomes. 
<img width="1065" height="460" alt="image" src="https://github.com/user-attachments/assets/a6a977d4-cb11-492d-a9fa-9e5f3d5c76cb" />

## Conclusion
**Context:** <br>
This project examined how major U.S. immigration policy shifts changed border enforcement outcomes from 2015 to 2025. Rather than relying only on raw totals, we compared repatriations, encounters, and efficiency ratios to understand whether policies improved enforcement results or simply changed processing volume. <br>
**Story:** <br>
Our analysis found that Title 42 was associated with higher repatriation counts, and nearly three-fourths of repatriations during that period were Title 42 expulsions. However, encounters increased even faster, causing the repatriation-to-encounter efficiency ratio to decline over time. This suggests the surge reflected a faster processing mechanism and higher activity levels, but not a lasting improvement in enforcement efficiency. The models reinforced this pattern, showing modest count increases under Title 42 but limited gains in the ratio itself. <br>
**Call to Action:** <br>
This research shows why policy outcomes should be evaluated using both totals and efficiency metrics, not raw counts alone. Future immigration policy decisions should focus on sustainable capacity, processing effectiveness, and long-term operational results rather than short-term spikes in reported enforcement numbers. For voters and the broader public, this research highlights the importance of evaluating immigration claims with complete metrics, not isolated totals. Informed civic decisions require asking whether policies improved long-term capacity, efficiency, and outcomes rather than only producing short-term spikes in reported numbers.

## Additional Adjacent Research:
- FY2019 Spike in Encounters. 
  - Due to push and pull effect (increased strife and poverty along with increased processing times)
- ICE Detentions over the past decade.
  - Detention durations have skyrocketed during and after the first Trump administration (likely due to policies such as MPP that impacted immigration court system processing time)
- Impacts of seasonal impacts.
  - There are consistent peaks in March and dips in December every year, likely indicating holiday-based impacts.
 
### Sources:
[1] [DHS – Repatriations](https://ohss.dhs.gov/khsm/dhs-repatriations) <br>
[2] [DHS – CBP Encounters](https://ohss.dhs.gov/khsm/cbp-encounters) <br>
[3] [CBP Encounters Data](https://www.cbp.gov/document/stats/nationwide-encounters) <br>
[4] Policy Marker (Used from [White House Policy Archive](https://www.whitehouse.gov/)) <br>
[5] [White House Official Website](https://www.whitehouse.gov/) <br>
[6] [TIME: Border Emergency & Military Involvement](https://time.com/5938570/border-emergency-military/) <br>
[7] [HHS: COVID-19 Public Health Emergency](https://www.hhs.gov/coronavirus/covid-19-public-health-emergency/index.html) <br>
[8] [CDC: Title 42 Legal Authorities (Archived Orders)](https://www.cdc.gov/port-health/legal-authorities/archived-orders.html) <br>
[9] [DHS: Mayorkas Statement on Ending Title 42](https://www.dhs.gov/archive/news/2022/04/01/statement-secretary-mayorkas-cdcs-title-42-order-termination) <br>
[10] [American Immigration Council: Guide to Title 42 Expulsions](https://www.americanimmigrationcouncil.org/fact-sheet/guide-title-42-expulsions-border/) <br>
[11] [Federal Register: Circumvention of Lawful Pathways Rule](https://www.federalregister.gov/documents/2023/05/16/2023-10146/circumvention-of-lawful-pathways) <br>
[12] [American Immigration Council: Migrant Protection Protocols (MPP)](https://www.americanimmigrationcouncil.org/fact-sheet/migrant-protection-protocols/) <br>
[13] [DHS: Reinstatement of Migrant Protection Protocols](https://www.dhs.gov/news/2025/01/21/dhs-reinstates-migrant-protection-protocols) <br>
[14] [DHS: 2021 Immigration Enforcement Priorities](https://www.dhs.gov/archive/news/2021/09/30/secretary-mayorkas-announces-new-immigration-enforcement-priorities) <br>
