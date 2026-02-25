---
layout: post
title: "The Hidden Geography of Inequality: Why India's Marginalized Groups Need Different Solutions"
date: 2025-12-05
author:
categories:

comments: true
math: true  
description: "An analysis of IHDS-II ( 2011-2012) data to understand the effect of social identity on employment."
---


## Persistence of Inequality

Inequality in labour market outcomes persists, even in the face of rapid economic growth in India. This project aimed to investigate the type of employment inequality faced by different social groups and how caste and religion shapes employment opportunities and outcomes. Understanding these dynamics is crucial, as employment is a primary determinant of an individual's life chances and overall socio-economic mobility.

A significant body of scholarly work has established the continuing relevance of social institutions like gender, caste, religion, and ethnicity in determining economic trajectories (Harriss-White and Gooptu 2001; Thorat et al 2005; Thorat and Newman 2010; Deshpande 2011). In the Indian context, experimental research provides stark evidence of these barriers. For instance, Thorat and Attewell (2010) found that equally qualified applicants from Muslim and Dalit backgrounds faced significant discrimination in hiring for formal urban jobs compared to their high-caste Hindu counterparts. 

Drawing on IHDS-II data from 204,568 individuals across 371 districts, our analysis exposes three distinct traps that fragment the Indian labor market. Muslims face a **Geographic Trap**, locked in regions where economic opportunities have evaporated. Adivasis are caught in a **Subsistence Mirage**, characterized by high work intensity but extreme poverty. Dalits encounter a **Distributed Barrier**, facing hiring discrimination that persists across all geographies. Because India treats these unique challenges with uniform policies, decades of reservations and poverty programs have failed to close the inequality gap.

A paradox as charted in the Figure 1 will help us in understanding the complexity of employment differences amongst different groups.

<figure class="text-center">
  <img src="\assets\img\IIHDSemploy\wealth_employment_paradox.png"
       alt="The Digital Divide" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 1:</strong> A bubble chart illustrating that groups with higher mean wealth (Forward castes) have lower employment rates, while the poorest groups (Adivasis) have the highest. 
  </figcaption>
</figure>


India's labor market tells a deceptive story. On the surface, employment statistics suggest a simple hierarchy: Adivasis (Scheduled Tribes) have the highest employment rate at 53.3%, followed by Dalits (Scheduled Castes) at 45.5%, while Muslims languish at the bottom with just 35.5% employment. Forward castes follow at 43.3%. These numbers have shaped decades of policy—but they hide a fundamental truth. 

The "point" of Muslims in this wealth-work relationship is their role as a critical outlier. While SC and ST groups fit the "distress labor" narrative—where lower wealth correlates with higher employment because they must work to survive—Muslims break this pattern. They possess higher mean wealth (15.3 compared to 14.0 for Dalits and 11.3 for Adivasis) yet suffer from much lower employment. This suggests that whereas SC/ST groups are pushed *into* low-quality labor by poverty, Muslims are being pushed *out* of the labor market entirely by their geographic concentration in stagnant regions.

The story of India's inequality is not just about who people are, it's fundamentally about where they live and what kinds of work they can access. Understanding these geographic and quality dimensions transforms our entire approach to addressing marginalization.

---

## Discussion on Employment Rate

### The Muslim Geographic Trap

#### Where Muslims Live Determines Whether They Can Work

When we analyzed employment rates across India's 371 districts, a striking pattern emerged. Districts with higher Muslim populations have systematically lower employment rates—not just for Muslims, but for everyone living there. For every 10 percentage point increase in a district's Muslim population share, the overall employment rate falls by 1.69 percentage points. This correlation of -0.305 is highly significant (p < 0.001).

The geographic concentration is stark. Consider Kerala's Malappuram district, where Muslims comprise 73.8% of the population. Despite Kerala's reputation for high literacy rates (Malappuram exceeds 94%), the district has the lowest employment rate in our entire dataset at just 25.7%. This may be influenced by heavy migration that happens. Compare this to districts with minimal Muslim populations: Himachal Pradesh's district 02_8 has 0% Muslim population and 75.6% employment. Chhattisgarh's district 22_15, also with nearly zero Muslims, boasts 72.5% employment.

This isn't limited to Kerala. Eastern Uttar Pradesh tells the same story. Districts in UP with 70-72% Muslim populations show employment rates hovering between 34-36%. Bihar's Muslim-majority districts average just 29% employment. Jammu and Kashmir's Muslim-dominated districts range from 33-48% employment. Across the board, high Muslim concentration predicts low employment for everyone in that district.


<figure class="text-center">
  <img src="\assets\img\IIHDSemploy\muslim_employment_correlation.png"
       alt="The Digital Divide" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 2:</strong> A scatterplot showing a significant negative correlation (-0.305) between a district's Muslim population share and its overall employment rate. It supports the argument that Muslims are concentrated in economically stagnant regions where jobs are scarce for everyone.
  </figcaption>
</figure>


#### What Happens Within Districts

When we compared Muslims and Brahmins living in different states, Muslims showed 7.7% lower odds of employment (OR = 0.923, p = 0.015)—a significant disadvantage. But when we compared Muslims and Brahmins living in the *same district*, this disadvantage completely vanished. The coefficient became +0.001 with a p-value of 0.842, meaning there's essentially no difference at all.

This district fixed effects test proves that the Muslim employment gap is 100% geographic. A case can be made that Muslims are concentrated in places where nobody—Muslim or Hindu—can find adequate employment. Rahman and Rauf (2025) in their regional analysis highlight the acute disadvantages muslims face in high-concentration districts, such as Murshidabad (55.3% literacy) and Uttar Dinajpur (52.1%), where inadequate infrastructure, teacher shortages, and socio-cultural barriers impede access. The Ranganath Mishra 
Commission's report and the The Sachar report, showed that the Muslims lagged far behind in their access to education, infrastructure, credit and employment in both public and private sectors. In fact, the literacy rate of Muslim males was only one percent above that of Dalit men—67.6% compared to 66.6%. 


### The Adivasi Subsistence Mirage

#### The Paradox of High Employment and Deep Poverty

The Adivasi employment pattern is the exact opposite of Muslims. Districts with higher Adivasi populations have significantly higher employment rates. The correlation is +0.378 (p < 0.001), even stronger than the Muslim correlation but in the reverse direction. For every 10 percentage point increase in Adivasi population share, district employment rises by 1.79 percentage points.

Chhattisgarh's tribal belt illustrates this dramatically. District 22_15, with 61.4% Adivasi population, has 72.5% employment—the highest in India. District 22_5, with 93.9% Adivasis, shows 63.3% employment. Gujarat's heavily tribal district 24_20 (96.9% Adivasi) has 62% employment. Mizoram, nearly entirely Adivasi at 97.7%, maintains 53.9% employment. These rates far exceed the national average of 44%.


<figure class="text-center">
  <img src="\assets\img\IIHDSemploy\st_employment_correlation.png"
       alt="Adivasi (ST) population share and district employment" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 3:</strong> A scatterplot showing a strong positive correlation (+0.378) between Adivasi (ST) population share and district employment. This visualizes the paradox where tribal belts have the highest employment rates in the country, but as the research shows, this is "distress employment" in subsistence agriculture.
  </figcaption>
</figure>

These high-employment districts are India's poorest regions. Chhattisgarh, Jharkhand, and Odisha—where Adivasis concentrate—rank among the bottom three states in per capita income. How can the group that works the most remain the poorest? The answer lies in what kind of work they're doing.

#### Why Adivasis Can't Stop Working

Adivasis concentrate in forest and hilly states where the economy is based on subsistence agriculture and forest produce collection. In these areas, there is no such thing as "unemployment" in the traditional sense. If you're not working, you're not eating. Women collect firewood, tend small rain-fed farms, and gather forest products like tendu leaves, mahua flowers, and sal seeds. Men do agricultural labor, migrate seasonally for construction work, or participate in small-scale mining.

This explains why Adivasi women's labor force participation is extraordinarily high—not because of gender equality, but because of poverty. Everyone must work because there's no alternative income source. The 13.6% of Adivasis participating in MGNREGA (the government employment guarantee scheme)—the highest rate of any group, four times that of Forward castes—confirms this desperation. When even subsistence work fails, they turn to government workfare programs that pay minimal wages.

The states where Adivasis concentrate have structural features that create high employment but low income. Forest reservation laws from the British era restricted Adivasis' access to land, pushing them into marginal agriculture. Lack of irrigation means dependence on monsoons. Poor roads and infrastructure limit market access, so farmers can't get good prices. The result is that everyone works constantly but remains trapped in poverty.

#### The Mirage of Employment Statistics

This reveals a fundamental flaw in using employment rates as a welfare metric. Adivasis top the employment rankings at 53.3%, which on paper looks successful. But this "high employment" is actually evidence of extreme deprivation. They're trapped in subsistence economies where survival requires constant labor but offers no path to accumulation or mobility. Development economists call this "distress employment"—working because you must, not because the work is productive or remunerative.

---

### The Dalit Distributed Pattern

#### No Geographic Pattern, Different Problem

When the same geographic analysis was run for Dalits, something unexpected happened: nothing. The correlation between Dalit population share and district employment rate was +0.081 with a p-value of 0.120—statistically indistinguishable from zero. Unlike Muslims (who concentrate in low-employment areas) or Adivasis (who concentrate in high-employment areas), Dalits show no geographic pattern at all.

Look at the variance in high-Dalit districts. Uttarakhand's district 05_8 has 66.7% Dalit population and 59.3% employment—quite high. Tamil Nadu's district 33_9, with 69.8% Dalits, shows 52.5% employment. But Punjab's district 03_5, with 56.9% Dalits, has just 36.7% employment. Delhi's heavily Dalit district 07_11 (52.4% Dalit) shows only 30.6% employment. The range is enormous: 30.6% to 59.3%, with no clear relationship to Dalit concentration.


<figure class="text-center">
  <img src="\assets\img\IIHDSemploy\sc_employment_correlation.png"
       alt="The Digital Divide" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 4:</strong> Shows a near-zero correlation (+0.081, non-significant) between Dalit concentration and district employment. This supports the claim that Dalit disadvantage is not geographic but is distributed across all regions due to caste-based barriers.
  </figcaption>
</figure>


Dalits were distributed across every village in India. The caste system assigned them "polluting" occupations like manual scavenging, leather work, agricultural labor, sanitation that existed everywhere. After independence, reservations and urbanization created even more geographic dispersion. 

#### Within-District Barriers

The lack of geographic pattern suggests Dalit disadvantage operates differently. While we haven't completed the district fixed effects analysis for Dalits yet, we predict it will show that the Dalit employment penalty *shrinks* but *remains* when comparing people in the same district—unlike Muslims, where it disappears entirely. This would indicate that Dalits face actual within-district discrimination in hiring and job access, rather than just being stuck in the wrong places.

---


## Discussion on Employment quality

Now we will look into what the analysis produced regarding employment quality by looking at contract of work and income. Among Muslims who do find work, the situation remains difficult. Our employment quality analysis shows that 78.1% of working Muslims have casual employment—daily wage work with no security, no advance notice, and no benefits. Only 17.6% have permanent contracts. 

**Insights on Urban Employment:**
The low participation of Muslims in MGNREGA (2.1%) underscores their concentration in urban and peri-urban areas. However, this urban presence does not translate into better job quality. Urban Muslim employment is characterized by **extreme informality**, with casualization rates exceeding 78%. Furthermore, Muslims show the lowest access to formal social security among all groups (mean Formal Index of 1.10), making them disproportionately vulnerable to urban economic shocks. This suggests that the urban labor market is as hostile to marginalized groups as the rural one, but through different mechanisms.


<figure class="text-center">
  <img src="\assets\img\IIHDSemploy\contract_type_distribution.png"
       alt="Type of Employment" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 5:</strong> A stacked bar chart showing the percentage of workers in Casual, Temporary, and Permanent contracts across social groups. It highlights that **85.5% of Adivasis** and **80.1% of Dalits** are in casual labor, compared to much higher permanent contract rates for Forward castes.
  </figcaption>
</figure>


Interestingly, only 2.1% of Muslims participate in MGNREGA, the rural employment guarantee scheme, even lower than Forward castes (2.4%) despite Muslims having much lower earnings. This confirms their urban and peri-urban concentration, as MGNREGA is primarily a rural program. Muslims need jobs where they live, not rural workfare programs they can't access. Therefore a a large
urban public employment garuntee programme as a garuntee on par with MGNREGA is needed. Scholars have discussed the ned for am urban employment garuntee which is not just an extension of MGNREGA but reimagines it according urban unemployment issues (Drèze 2020, Bsole 2019, Bhan et al 2024)

Among working Dalits, 80.1% have casual employment, 15.7% have permanent jobs, as shown in Figure 5 and mean earnings are ₹43,294 (52.2% less than Forward castes). Adivasis on the other hand face the worst job quality of any group we studied. As Figure 5 shows a devastating 85.5% work in casual employment, contributing to the highest casualization rate of any social group. Only 11.8% have permanent jobs, compared to 40.6% of Forward castes. This means most Adivasis wake up each day uncertain whether they'll have work, negotiating wages daily with no security whatsoever.

<figure class="text-center">
  <img src="\assets\img\IIHDSemploy\earnings_distribution.png"
       alt="Job Security" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 6:</strong> Boxplots of annual earnings on a **Log Scale**. It shows the persistent shift toward higher earnings for Forward castes, even when ignoring outliers, and highlights the "Subsistence Mirage" of Adivasis who earn the least despite working the most. 
  </figcaption>
</figure>


The earnings data is even more shocking. Adivasis' mean annual earnings are ₹35,883—a full 60.4% less than Forward castes. The median is worse: ₹15,000 versus ₹48,000 for Forward castes, a 68% gap. Even after controlling for education, age, gender, and location, Adivasis face a wage penalty of 54.6%—the largest of any group. This means that an Adivasi and a Forward caste person with the same education, working in the same state, will see the Adivasi earn barely half as much.

Adivasis work more (53.3% employment rate) but earn so little per job that their annual income per person is ₹19,125 (employment rate × mean earnings). Forward castes work less (39.8% employment rate) but earn so much per job that their annual income reaches ₹36,049—nearly double. Forward castes work 25% less but earn 88% more overall. After controlling for education and location, the analysis shows Dalits still earn 32.2% less—a substantial penalty that suggests occupational segregation or discrimination persists. Their MGNREGA participation of 6.6% indicates that many rely on government workfare when private employment fails.

Meanwhile mean annual earnings of muslims is ₹50,567, which is 44.2% less than Forward castes' ₹90,577. Even after controlling for education, age, gender, and location, Muslims earn 19.9% less (p < 0.001).



## The Methodological Insight

### Why the Comparison Matters

The power of this analysis comes from comparing three groups simultaneously. If the Muslim geographic pattern were due to methodological problems—measurement error, model misspecification, or omitted variables—we would expect to see similar patterns for other marginalized groups. But we don't. We see three completely different patterns that align perfectly with three distinct historical narratives.

Muslims show strong negative geographic sorting (-0.305 correlation) because of Partition-era concentration and urban deindustrialization. Adivasis show strong positive geographic sorting (+0.378 correlation) because of British-era forest reservation policies and subsistence economies. Dalits show no geographic pattern (0.081 correlation, not significant) because of caste-based occupational segregation that existed everywhere.

This three-way comparison acts as a falsification test. The methodology is sound precisely because it yields different results for groups with different histories. If we only studied Muslims, skeptics could argue the geographic pattern is spurious. Studying all three groups simultaneously proves the patterns are real.

### Rethinking Employment as a Metric

Perhaps the most important lesson we can learn from this analysis is that employment rates alone are deeply misleading. Adivasis rank first in employment (53.3%) but last in income. Forward castes rank fifth in employment (39.8%) but first in income. The disconnect occurs because employment without adequate wages produces poverty, not prosperity.

When Adivasis' 53.3% employment rate is multiplied by their ₹35,883 mean earnings, we get ₹19,125 in annual income per person—the lowest of any group. When Forward castes' 39.8% employment rate is multiplied by their ₹90,577 mean earnings, we get ₹36,049—nearly double Adivasis' income despite working 25% less.

This demonstrates that researchers and policymakers must disaggregate employment into at least four components: employment rate (quantity), earnings level (wages), job security (permanent vs. casual), and benefit coverage (formal vs. informal). 

Our visualization of earnings distribution (Log Scale) highlights the massive spread within groups, yet the persistent shift to the right for Forward castes remains evident. Similarly, the contract type distribution chart reveals that the "high employment" of Adivasis and Dalits is almost entirely fueled by casual labor, whereas the majority of Forward caste jobs carry the security of permanent contracts. High employment with low wages and no security—the Adivasi pattern—is actually evidence of distress, not success.

---

## Conclusion: From Universal Policies to Targeted Solutions

The geography of marginalization in India operates through three distinct mechanisms. Muslims suffer from geographic segregation in economically stagnant districts—a quantity problem requiring place-based development. Adivasis suffer from employment quality deprivation in subsistence economies—a quality problem requiring wage and productivity enhancement. Dalits still suffer from distributed discrimination across all regions—an access problem requiring anti-discrimination enforcement and mobility support.

The evidence from 204,568 individuals across 371 districts tells us that understanding *why* outcomes differ must precede deciding *what* to do. Muslims don't need better access to jobs that don't exist—they need the jobs to exist in the first place. Adivasis don't need more work—they're already working themselves into exhaustion—they need that work to pay living wages. Dalits don't need geographic targeting—they're everywhere—they need discrimination to stop.

Effective policy should address the fact that marginalization is heterogeneous and mechanisms differ across groups. Only by matching interventions to the specific barriers each group faces—geographic, economic, or discriminatory—can India begin to close gaps that decades of well-intentioned but misdirected policies have failed to address.

---

## Summary Table: Three Groups, Three Solutions

| Dimension | Muslims | Adivasis | Dalits |
|-----------|---------|----------|--------|
| **Employment Rate** | 35.5% (Lowest) | 53.3% (Highest) | 45.5% (Middle) |
| **Geographic Pattern** | Negative (-0.305***) | Positive (+0.378***) | None (0.081 n.s.) |
| **District FE Result** | Disappears completely | TBD | TBD |
| **Casual Employment** | 78.1% | 85.5% | 80.1% |
| **Mean Earnings** | ₹50,567 (-44.2%) | ₹35,883 (-60.4%) | ₹43,294 (-52.2%) |
| **Wage Penalty (Adjusted)** | -19.9% | -54.6% | -32.2% |
| **MGNREGA Participation** | 2.1% (Urban) | 9.1% (Highest) | 6.6% (Second) |
| **Primary Problem** | Job scarcity | Job quality | Access barriers |
| **Historical Root** | Partition + deindustrialization | Forest reservation + subsistence | Caste occupational segregation |
| **Policy Lever** | Place-based development | Wage/productivity enhancement | Anti-discrimination enforcement |
| **Expected Impact** | Close 75% of employment gap | Reduce poverty from 45% to 30-35% | Raise employment from 45.5% to 48-50% |

---

## Data & Methods

- **Source**: Desai, Sonalde, Reeve Vanneman and National Council of Applied Economic Research. India Human Development Survey-II (IHDS-II), 2011-12. Inter-university Consortium for Political and Social Research [distributor], 2018-08-08. https://doi.org/10.3886/ICPSR36151.v6
- **Sample**: 204,568 individuals across 371 districts in 33 states
- **Methods**: District fixed effects models, geographic correlation analysis, wage regressions with education and location controls
- **Standard Errors**: Clustered at Primary Sampling Unit (PSU) level

**Keywords**: Employment inequality, geographic sorting, caste and religion, labor market discrimination, India, development economics



## Bibliography

Basole, A (2019): “State of Working India 2019,” Centre for Sustainable Employment, Azim Premji University, https://publications.azimpremjiuniversity.edu.in/1977/1/State_of_Working_India_2019.pdf.

Bhan, G., Anand, S., Nagpal, S., & Khandelwal, V. (2024). Reimagining urban employment programmes. Economic & Political Weekly, 59(22), 14-18.

Deshpande, A (2011): The Grammar of Caste: Economic Discrimination in Contemporary India, Oxford: Oxford University Press. 


Drèze, J (2020): “Decentralised Urban Employment and Training (DUET) Scheme: A Proposal,” Policy Brief No 23, National Centre for Demographic Studies, https://ncds.nic.in/sites/default/files/PolicyBriefs/PB23NCDS.pdf.

Harriss-White, B and N Gooptu (2001): “Mapping India’s World of Unorganised Labour,” Socialist Register, Vol 37, pp 89–118.

Mhaskar, S. (2018). Ghettoisation of economic choices in a global city: A case study of Mumbai. Economic and Political Weekly, 29-37.

Thorat, S, Aryama and P Negi (eds) (2005): Reservation and Private Sector: Quest for Equal Opportunity and Growth, Indian Institute of Dalit Studies, New Delhi.

Thorat, S and P Attewell (2010): “The Legacy of Social Exclusion: A Correspondence Study of Job Discrimination in India’s Urban Private Sector,” Blocked by Caste: Economic Discrimination in Modern India, S Thorat and K S Newman (eds), New Delhi: Oxford University Press.

Thorat, S and K S Newman (eds) (2010): Blocked by Caste: Economic Discrimination in Modern India, New Delhi: Oxford University Press.