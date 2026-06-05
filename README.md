# 🎯 The Sugar Trap — Market Gap Analysis
### Submission by: Lawrence Koomson | BSc. IT — Data Science & Analytics | UCC 2026
### Client: Helix CPG Partners | AmaliTech Capstone Challenge 2026

---

## A. Executive Summary

Analysis of 109,564 food products from the Open Food Facts database reveals
a clear and actionable market gap in the healthy snacking space. The snack
market is heavily oversaturated with High Sugar + Low Protein products
(11,946 products), while the Blue Ocean of High Protein + Low Sugar remains
underserved despite strong consumer demand for healthier options.

The biggest market opportunity lies in the Dairy & Eggs category, where
products averaging 20.2g of protein and just 2.5g of sugar per 100g exist
but are not being actively developed as consumer snack products. Health
validation using Nutri-Score confirms Blue Ocean products score A/B
(healthy) while 54.1% of oversaturated products score E (worst) — proving
the gap is real, measurable and actionable.

R&D teams should focus on Soy/Soya, Peanuts and Whey as the top three
protein sources driving high-protein product performance in the current
market.

---

## B. Project Links

- **Notebook:** [Google Colab — AmaliTech Market Gap Analysis](https://colab.research.google.com/drive/1yqRwxSJzK68tQU7KMyR-HQZTOZzcl2eo?usp=sharing)
- **Dashboard:** [Live Dashboard — Looker Studio](https://datastudio.google.com/reporting/3658f873-fed3-49b0-959e-6c950392e7c1)
- **Presentation:** [Slide Deck — Google Slides](https://docs.google.com/presentation/d/1mrB46Uew1bit1C0PbzkABV9D5sW382pfphQOwjCegmw/edit?usp=sharing)

---

## C. Technical Explanation

### Data Cleaning Approach
Starting from 500,000 raw rows I applied a 4-step cleaning pipeline:
1. Removed rows with missing product_name — 15,790 rows removed
2. Removed rows missing both sugars_100g AND proteins_100g — 374,384 rows removed
3. Filtered biologically impossible outliers where any nutrient exceeded
   100g per 100g — 200 rows removed
4. Removed rows where combined macronutrients exceeded 105g per 100g —
   62 rows removed

**Final clean dataset: 109,564 rows — reliable and analysis-ready.**

### Candidate's Choice — Nutri-Score Health Validation
I added a Nutri-Score (A-E) health rating comparison between Blue Ocean
products and the Oversaturated zone. This was added because the client
needs to know not just WHERE the market gap is, but whether those products
are genuinely healthy by an independent scientific standard.

The finding — Blue Ocean products score 24.5% A (Best) while oversaturated
products score 54.1% E (Worst) — provides powerful evidence for premium
health positioning in Helix CPG Partners go-to-market strategy.

---

## D. Key Findings

| Finding | Value |
|---|---|
| Total products analysed | 109,564 |
| Blue Ocean products (High Protein + Low Sugar) | 11,869 |
| Oversaturated products (High Sugar + Low Protein) | 11,946 |
| Best opportunity category | Dairy & Eggs |
| Target protein | 20.2g per 100g |
| Target max sugar | 4.3g per 100g |
| #1 Protein source | Soy/Soya (30.3%) |
| #2 Protein source | Peanuts (9.7%) |
| #3 Protein source | Whey (9.0%) |

---

## E. Technology Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computing |
| Matplotlib & Seaborn | Data visualization |
| Google Colab | Cloud notebook environment |
| Google Looker Studio | Interactive dashboard |
| Open Food Facts | Dataset source |
| GitHub | Version control and submission |

---

## F. Repository Contents

| File | Description |
|---|---|
| AmaliTech_Market_Gap_Analysis.ipynb | Main Jupyter notebook |
| AmaliTech_Market_Gap_Analysis.html | HTML export of notebook |
| AmaliTech_Complete_Dashboard.png | Complete analysis dashboard |
| story1_distributions.png | Data cleaning distributions |
| story2_categories.png | Category distribution chart |
| story3_nutrient_matrix.png | Sugar vs Protein scatter plot |
| story4_recommendation.png | Market quadrant analysis |
| story4_key_insight_box.png | Key insight visualization |
| story5_hidden_gem.png | Top protein sources chart |
| story6_candidates_choice.png | Nutri-Score comparison |
| story6_nutriscore_heatmap.png | Nutri-Score by category heatmap |

---

## G. Pre-Submission Checklist

- [x] GitHub Repo is Public
- [x] .ipynb notebook uploaded
- [x] HTML export uploaded
- [x] Raw dataset NOT uploaded
- [x] Code uses relative paths
- [x] Dashboard publicly accessible
- [x] Presentation publicly accessible
- [x] README updated with Executive Summary
- [x] Stories 1-4 completed
- [x] Candidate's Choice completed and explained
