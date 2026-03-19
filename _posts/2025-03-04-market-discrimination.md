---
layout: post
title: "Market Access and Price Discrimination in Indian Agriculture"
date: 2026-01-19
categories: 

comments: true
math: true
description: "An analysis of NSS 77th Round (2019) data to understand the effect of social identity on agricultural market access and price returns."
---

<div class="text-center mt-4 mb-4">
  <a href="https://github.com/ashwinnsr/agricultural-market-discrimination" 
     class="btn btn-primary" 
     target="_blank" 
     rel="noopener noreferrer">
    <i class="fab fa-github"></i> View Code on GitHub
  </a>
</div>

## Abstract
In the discourse on agrarian inequality in India, attention is typically directed toward land ownership, credit monopolies, and debt cycles. However, the final frontier of the agricultural cycle—the market exchange—remains deeply stratified by social identity. This article leverages the National Sample Survey (NSS) 77th Round (2019) to analyze over 39,219 crop sales records, examining how caste and tribal identities dictate terms of trade. Utilizing high-dimensional fixed-effects models and quantile regressions, we find that Scheduled Caste (SC) and Scheduled Tribe (ST) farmers face significant structural penalties. SC farmers are 10.5 percentage points less likely to sell to private informal traders but face a persistent "glass ceiling" in price returns, being locked out of premium market rates. Conversely, ST farmers suffer from extreme geographic isolation and "adverse incorporation" through tied land-labor arrangements (sharecropping), which imposes a devastating 23.3% price penalty. We argue for a paradigm shift from prioritizing physical market access to dismantling pre-market socio-economic dependencies.

---

## 1. Research Problem
When a farmer brings their harvest to the market, economic theory suggests that the price should be dictated by supply, demand, crop quality, and volume. However, rural Indian markets are embedded within rigid socio-economic hierarchies. While significant literature has established the existence of caste-based discrimination in labor and credit markets, less empirical attention has been paid to the product market—specifically, the prices farmers receive for their crops and the agencies they sell to.

The core research problem addresses the persistent illusion that "market entry" equates to "market equality." Marginalized farmers—particularly Dalits (Scheduled Castes) and Adivasis (Scheduled Tribes)—are actively participating in agricultural markets, yet their agrarian distress remains disproportionately high. If they are accessing formal and informal markets, why does the value they extract from their harvest remain fundamentally depressed? This project aims to unpack the opaque mechanisms of market discrimination that operate even when geographic and spatial variables are held constant.

---

## 2. Research Questions
This analysis is driven by two primary research questions:
1. **The Market Inclusion Squeeze (H1):** Do Scheduled Caste (SC) and Scheduled Tribe (ST) farmers face systemic price discrimination when selling identical crops, in identical volumes, within the exact same districts as their General Caste counterparts? If so, does this penalty apply uniformly across the price spectrum, or is it concentrated at specific extremes?
2. **The Agency Access Squeeze (H2):** Are historically marginalized farmers systematically excluded from specific market channels (e.g., formal government procurement processes or lucrative private traders) due to their social identity?

---

## 3. Methodology
This research utilizes the unit-level data from the **NSS 77th Round (2019) "Situation Assessment of Agricultural Households"**, constituting a final analytical dataset of 39,219 distinct crop sales. To rigorously isolate the effect of social identity from confounding economic factors, the following methodologies were employed:

*   **Fixed Effects OLS Models:** To neutralize geographic variation, the baseline econometric model implements strict District Fixed-Effects alongside Crop Fixed-Effects. This ensures that an SC farmer is only being compared to a General Caste farmer selling the *exact same crop* in the *exact same district*. We further controlled for household wealth (using Log Monthly Per Capita Expenditure) and total landholdings.
*   **Quantile Regressions (`rq`, Frisch-Newton Method):** Ordinary Least Squares (OLS) calculates the "average" penalty. To see how discrimination operates at the extremes (distress sales vs. premium sales), we ran quantile regressions at the 10th, 50th, and 90th percentiles.
*   **Linear Probability Models (LPM):** To measure market agency choice, we modeled the probability of selling to specific channels (Private Traders, Mandis, Government/FCI, and Cooperatives) against social identity.
*   **Mechanism Proxies (Adverse Incorporation):** We tested interaction terms between caste and lease arrangements (sharecropping) to quantify the price penalty exerted by interlocked land-labor markets.

*(All data cleaning, spatial merging, and econometric modeling were conducted in R utilizing the `fixest` and `quantreg` packages).*

---

## 4. Results
The empirical output shatters the assumption of market neutrality, revealing layered, structural traps that penalize marginalized farmers.

### 4.1 Divergent Market Access (The Agency Squeeze)
The clearest divergence in the dataset is *who* farmers sell to:
*   **The SC Retreat from Private Markets:** SC farmers are structurally retreating from informal, private traders. Our models show a highly significant **-10.5 percentage point drop** in the probability of SC farmers selling to private traders compared to General Caste farmers. 
*   **The Government Void:** Despite avoiding private traders, SC and ST farmers do not meaningfully capture state support. The likelihood of selling to Government Procurement (FCI) or Cooperatives sees a minuscule, statistically insignificant boost (`+0.001` coefficient). They are effectively squeezed out of both lucrative private networks and protective state channels.


<figure class="text-center">
  <img src="\assets\img\agriculture-discrimination\market_access_by_caste_expanded.png"
       alt="Bar chart showing a systematic retreat from private informal traders by marginalized farmers" 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
     <strong>Figure 1:</strong> Market Access Divergence. A visual representation demonstrating that SC farmers are 10.5 percentage points less likely to sell to private informal traders compared to General Caste farmers.
  </figcaption>
</figure>


### 4.2 The Glass Ceiling of Price Returns
Are SC farmers getting lower prices on average? Yes. The robust District-Fixed Effects model identifies a consistent **2.3% baseline price penalty** for SC farmers. However, the Quantile Regression results provide the most revolutionary insight: the penalty is not universal; it is heavily skewed toward the top.

<figure class="text-center">
  <img src="\assets\img\agriculture-discrimination\price_gaps_by_caste.png"
       alt="Bar chart comparing average agricultural price returns by social group, demonstrating lower absolute returns for SC and ST farmers." 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
     <strong>Figure 2:</strong> Baseline Price Returns. Marginalized farmers receive systematically lower prices for their crops, with SC farmers facing a robust 2.3% penalty even when geography and crop type are strictly controlled.
  </figcaption>
</figure>


*   **10th Percentile (Distress Sales):** At the absolute bottom of the market, there is no caste penalty. In fact, SC farmers show a negligible `+0.9%` coefficient. When the market collapses, it crushes everyone equally.
*   **90th Percentile (Premium Sales):** At the top of the market, where premium prices are paid for high-quality or perfectly timed crops, SC farmers face a massive **1.9% penalty**. 


<figure class="text-center">
  <img src="\assets\img\agriculture-discrimination\plot_marginal_penalty.png"
       alt="Point plot with confidence intervals showing the SC price penalty distributed across different farmer land size categories." 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
     <strong>Figure 3:</strong> The Penalty Variance. The severity of price discrimination experienced by Scheduled Caste farmers varies significantly across land ownership size classes.
  </figcaption>
</figure>

### 4.3 Adverse Incorporation and Sharecropping
Why does this penalty exist? We tested the hypothesis of "Adverse Incorporation"—the idea that marginalized farmers are forced to sell crops at artificially low prices to local landlords or creditors to pay back loans or access land.
*   **The Universal Sharecropper Penalty:** Operating as a sharecropper exerts a baseline **4.8% price penalty** across the board. 
*   **The ST Geography & Tenancy Trap:** For Adivasi (ST) farmers, the interaction between being a sharecropper and their tribal identity triggers a devastating **23.3% structural price penalty** (marginally significant, p=0.059). ST farmers, already suffering from geographic isolation, face extreme rural exploitation when locked into informal tenancy agreements.

<figure class="text-center">
  <img src="\assets\img\agriculture-discrimination\st_land_penalty_plot.png"
       alt="Point plot displaying the extreme price penalty faced by Scheduled Tribe farmers compared to Scheduled Caste farmers across land sizes when operating as sharecroppers." 
       class="img-fluid" 
       style="max-width: 85%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <figcaption class="mt-2 text-muted">
     <strong>Figure 4:</strong> The Tribal Sharecropper Squeeze. Adivasi (ST) sharecroppers face an extreme 23.3% structural price penalty, illustrating the compound effects of geographic isolation and informal tenancy.
  </figcaption>
</figure>

---

## 5. Discussion

The findings of this empirical analysis challenge the prevailing narrative of agrarian reform in India. For decades, policy interventions have focused almost exclusively on building more physical markets (Mandis), guaranteeing Minimum Support Prices (MSPs), and expanding road infrastructure under the assumption that "inclusion" is the final hurdle. 

Our results prove that inclusion without equity is merely a different form of extraction. 

SC farmers have successfully entered the formal market space (moving away from private traders), yet they have run face-first into a "glass ceiling." The quantile regressions demonstrate that the market does not discriminate during times of distress; rather, it actively excludes Dalit farmers from capturing premium, high-value returns. They can play the game, but they are systemically prevented from winning it.

Simultaneously, the staggering 23.3% price penalty faced by tribal sharecroppers confirms that agricultural markets are hopelessly interlocked with land and credit markets. When an ST farmer brings their crop to market, the price is not negotiated based on supply and demand; it is dictated by pre-existing social dependencies, debt obligations, and local power monopolies. This is the hallmark of *Adverse Incorporation*—they are included in the agrarian economy strictly on terms that extract their surplus value.

### Conclusion and Policy Implications
Agricultural markets are not neutral economic arbiters; they are arenas where pre-existing social hierarchies are enforced and monetized. 

If true agrarian equity is to be achieved, policymakers must recognize that the "Final Mile" of the crop sale is compromised before the farmer even leaves their village. Interventions that solely target market infrastructure will fail. Instead, reforms must aggressively target the root causes of Adverse Incorporation: dismantling interlocked tenancy monopolies, providing heavily subsidized, identity-blind institutional credit, and enforcing stringent anti-discrimination frameworks within APMC Mandis and Government Procurement systems. 

The double squeeze of restricted access and predatory pricing cannot be solved until the agrarian market is structurally decoupled from caste and tribal subjugation.

***
*All datasets, R-scripts, diagnostic files, and spatial mappings used in this analysis are open-source and available in the project GitHub repository.*
