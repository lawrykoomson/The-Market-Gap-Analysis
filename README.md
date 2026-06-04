# 🎯 THE SUGAR TRAP — Market Gap Analysis
### Submission by: Lawrence Koomson | BSc. IT — Data Science & Analytics | UCC 2026
### Client: Helix CPG Partners | AmaliTech Capstone Challenge 2026

---

## A. Executive Summary

Analysis of 109,564 food products from the Open Food Facts database reveals a clear
and actionable market gap in the healthy snacking space. The snack market is heavily
oversaturated with High Sugar + Low Protein products (11,946 products), while the
Blue Ocean of High Protein + Low Sugar remains underserved despite strong consumer
demand for healthier options.

The biggest market opportunity lies in the Dairy & Eggs category, where products
averaging 20.2g of protein and just 2.5g of sugar per 100g exist but are not being
actively developed as consumer snack products. Health validation using Nutri-Score
confirms Blue Ocean products score A/B (healthy) while 54.1% of oversaturated
products score E (worst) — proving the gap is real, measurable and actionable.

R&D teams should focus on Soy/Soya, Peanuts and Whey as the top three protein
sources driving high-protein product performance in the current market.

---

## B. Project Links

- **Link to Notebook:** [Google Colab Notebook](https://colab.research.google.com/drive/1yqRwxSJzK68tQU7KMyR-HQZTOZzcl2eo?usp=sharing)
- **Link to Dashboard:** [AmaliTech Complete Dashboard](https://github.com/lawrykoomson/The-Market-Gap-Analysis/blob/main/AmaliTech_Complete_Dashboard.png)
- **Link to Presentation:** [View Analysis Charts on GitHub](https://github.com/lawrykoomson/The-Market-Gap-Analysis)

---

## C. Technical Explanation

### Data Cleaning Approach
Starting from 500,000 raw rows, I applied a 4-step cleaning pipeline:
1. Removed rows with missing product_name (15,790 rows removed)
2. Removed rows missing both sugars_100g AND proteins_100g (374,384 rows removed)
3. Filtered biologically impossible outliers where any nutrient exceeded 100g per 100g (200 rows)
4. Removed rows where combined macronutrients exceeded 105g per 100g (62 rows)
Final clean dataset: 109,564 rows — reliable and analysis-ready.

### Candidate's Choice — Nutri-Score Health Validation
I added a Nutri-Score (A-E) health rating comparison between Blue Ocean products
and the Oversaturated zone. This was added because the client needs to know not
just WHERE the market gap is, but whether those products are genuinely healthy by
an independent scientific standard. The finding — Blue Ocean products score 24.5%
A (Best) while oversaturated products score 54.1% E (Worst) — provides powerful
evidence for premium health positioning in Helix CPG Partners' go-to-market strategy.

---
