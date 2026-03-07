---
layout: post
title: "The Mechanisms of Market Discrimination in Indian Agriculture"
date: 2025-03-04
---

Despite the modernization of Indian agriculture, caste-based disparities continue to dictate economic outcomes in the rural sector. Literature on caste-based analysis on Indian Agriculture revolve around income disparities, agricultural output and yield demonstrating the disadvantage that SC and ST face in agriculture (Deshpande 2000; Thorat et al 2007; Rawal and Swaminathan 2011; Agarwal and Mahesh 2021; Rao 2017). Studies also analyze caste disparities in access to credit,  quality information and landholding (Kumar and Venkatachalam 2019; Krishna et al 2019; Goli et al 2015). 

While historical discourse has largely focused on disparities in land ownership and access to credit, less attention has been paid to the final mile of the agricultural cycle: \textbf{market realization}. In addition, much of policy discussion and academic literature adopt a binary frame work of “disadvantaged” versus “upper caste” groups, often overlooking the differences among the disadvantaged groups, an omission with significant theoretical, empirical, and policy implications. Few studies focus specifi cally on caste disparities in agricultural net returns. 

The study demonstrates that Scheduled Caste (SC) and Scheduled Tribe (ST) farmers face distinct, rather than uniform, layers of economic disadvantage compared to General Caste farmers. Using micro-level data from the National Sample Survey (NSS) 77th Round (2019), we identify divergent mechanisms of exclusion. ST farmers face a \textbf{Market Access Bias}, remaining structurally dependent on informal private traders due to geographic isolation. Conversely, SC farmers successfully access formal markets but face an intersectional \textbf{Price Discrimination}. `Marginal'' SC farmers suffer a significant price penalty despite selling in regulated channels. This provides robust econometric evidence that barriers operate differently across social groups—via exclusion for Adivasis and via stratified valuation for the poorest Dalits—preventing them from realizing the full value of their agricultural labor

Our recent empirical analysis of the National Sample Survey (NSS) 77th Round (2019)—analyzing over 41,000 agricultural sales records across India—suggests the answer is a resounding no. By applying robust econometric methods, including District Fixed Effects to neutralize geographic variations, we uncovered that marginalized farmers face distinct, layered mechanisms of economic extraction, rather than a uniform disadvantage.

Here is a deep dive into the structural traps embedded in agrarian markets.

### The Illusion of Inclusion: The Market Access Divide
Our first objective was to understand who sells to whom. Do marginalized farmers rely more on informal private traders, while dominant castes dominate formal, regulated Mandis? 

The data reveals a stark divergence between Scheduled Caste (SC) and Scheduled Tribe (ST) farmers:

* **The Geographic Trap (ST):** Adivasi (ST) farmers remain structurally dependent on informal private traders (a 4.0% higher likelihood). This is highly consistent with theories of geographic isolation; remote farmers simply cannot physically access formal markets.
* **The SC Divergence:** In contrast, Dalit (SC) farmers are **10.1 percentage points less likely** to sell to private traders compared to General Caste farmers. They have successfully entered the formal market system, disproportionately utilizing regulated Mandis.

However, formal access does not mean equal treatment. Despite their presence in Mandis, SC farmers exhibit systematically lower access to premium, state-run Government Procurement (FCI) channels compared to their General Caste peers. 

<figure class="text-center">
  <img src="C:\Users\ashwin\Documents\Agrarian_ market acess\code\plots\market_access_by_caste_expanded.png"
       alt="The Invisible Workshop" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 1:</strong> Bar chart showing percentage of sales routed through different agencies (Trader, Mandi, Govt, Coop) by social group
  </figcaption>
</figure>


### Distributional Penalties: Who Really Pays the Price?
If SC farmers are reaching formal markets, are they getting formal prices? 

A standard average analysis (Ordinary Least Squares) suggests a negligible aggregate price penalty of just -0.7% for SC farmers. However, averages can be deceptive. When we applied **Quantile Regressions** to look across the entire price distribution (from distress sales to premium sales), a predatory gradient emerged:

* **Exclusion from Premium Markets (90th Percentile):** At the highest end of the market, SC farmers face a highly significant **-1.4% price penalty**. The most lucrative market opportunities remain disproportionately captured by dominant castes.
* **Equalization at the Bottom (10th Percentile):** At the bottom of the market (distress sales), the caste penalty disappears completely (+1.7%). This points to a grim universal price floor: when farmers are desperate, the market offers uniformly poor prices to everyone, regardless of caste.

<figure class="text-center">
  <img src="C:\Users\ashwin\Documents\Agrarian_ market acess\code\plots\price_gaps_by_caste.png" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 2:</strong> Bar chart showing average crop price by social group with confidence intervals
  </figcaption>
</figure>


### The Intersection of Caste and Class
Market discrimination is not a blanket phenomenon; it is fiercely intersectional. When we interacted social identity with landholding size, we found that wealthier SC farmers (Small, Medium, and Large) show no statistically significant price difference compared to General Caste peers in their district.

The burden falls entirely on the most vulnerable. **"Marginal" SC farmers (owning less than 0.5 hectares) face a severe 8.2% revenue loss** compared to General Caste neighbors selling in the same district. They are in the formal market, but they lack the bargaining power or social capital to realize fair value.


<figure class="text-center">
  <img src="C:\Users\ashwin\Documents\Agrarian_ market acess\code\plots\st_land_penalty_plot.png" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
    <strong>Figure 3:</strong> Line chart showing price penalty coefficients across different land size classifications for ST/SC groups
  </figcaption>
</figure>


### Beyond Geography: The Mechanisms of Adverse Incorporation
Why do these poorest farmers face penalties even when standing inside a regulated Mandi? The answer lies outside the market gates, in pre-existing socio-economic dependencies—a concept known as **Adverse Incorporation**.

To test this, we used sharecropping as a proxy for interlocked land and labor dependencies. The data confirmed a massive **Sharecropper Penalty**. Farmers operating under lease terms face significant price penalties compared to landowners selling the exact same crop in the exact same district. When a farmer is deeply indebted to a local landlord or trader for land or inputs, the terms of trade at harvest are already rigged against them. The physical location of the sale (Mandi vs. village) becomes irrelevant if the social relation dictates the price.

### Conclusion
Our analysis shatters the simplistic binary of "excluded vs. included." Agrarian markets fail marginalized communities through multi-layered structural traps. ST farmers face exclusion via geographic isolation, while SC farmers face *Adverse Incorporation*—they are included in the market, but strictly on terms that extract their surplus value.

For the smallest landholders, the market is not a neutral economic arbiter; it is a mechanism of stratified extraction. Policy interventions that merely focus on building more physical markets (Mandis) will fail to address the fundamental, pre-market power imbalances that dictate who gets paid what. True agricultural reform must address the interlocked dependencies of land, credit, and social identity that shape the final mile.

***
*Methodological Note: This analysis was built using R, leveraging `fixest` for District Fixed Effects and `quantreg` for distributional analysis. Scripts and replication data structures are available on my GitHub repository.*
