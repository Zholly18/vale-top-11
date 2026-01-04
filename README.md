# VALE Ads Monetization Analysis (Nordeus Case Study)

## Project overview
This project is a business & data analytics case study based on a test assignment from Nordeus.
The goal is to evaluate the effectiveness of a new advertising format (VALE ads) and to assess
whether VALE ads increase total revenue **without cannibalizing traditional ads or in-app purchases (IAP)**.

The analysis is based on aggregated user activity, advertising events, and monetization data.

---

## Business goals

### Goal 1 — VALE monetization impact
Evaluate whether VALE ads successfully:
- Engage active users who do not make (or rarely make) IAP purchases
- Generate incremental ad revenue
- Contribute positively to total revenue

### Goal 2 — Cannibalization check
Assess whether viewing VALE ads negatively affects:
- The number of traditional (regular) ads viewed
- Revenue from regular ads

---

## Data description

The analysis uses the following datasets:
- **User stories data** — user-level activity and IAP-related metrics
- **Ads data** — ad impressions, revenue, and ad type indicators
- **Data dictionary** — definitions of all variables provided in the task

Key entities:
- Users are identified by `global_user_id`
- Ad revenue is measured in USD
- VALE ads are identified based on the `reason` field pattern

---

## Analytical approach

### Data preparation
- Merged user-level and ad-level data
- Created derived metrics:
  - Total ads count
  - VALE ads count
  - Regular ads count
  - VALE revenue
  - Regular ads revenue
- Built user-level segmentation flags

### User segmentation
Users were segmented based on monetization and ad behavior:
- **Payers / Non-payers**
- **Regular ads only users**
- **VALE only users**
- **Mixed ads users (VALE + regular ads)**

---

## Key findings

### Goal 1 — VALE monetization
- VALE ads generate additional ad revenue
- VALE-only users represent a small but clearly monetizable segment
- Mixed users (VALE + regular ads) generate the highest ad revenue per user

### Goal 2 — Cannibalization
- Users who watch VALE ads also tend to watch **more regular ads**, not fewer
- No evidence of cannibalization at an aggregated level
- Initial results suggest complementary rather than competitive behavior between VALE and regular ads

---

## Data limitations

- No user-level temporal sequence (before / after VALE exposure)
- No explicit control group
- No experimental or A/B test design

As a result, **causal cannibalization effects cannot be confirmed**.
The analysis is limited to descriptive and comparative insights,
and observed differences should be interpreted as correlations rather than causal impact.

---

## Visualizations

The project includes:
- Revenue share breakdown (IAP vs ads vs VALE ads)
- Average ads watched per user by segment
- Comparative visualizations to support cannibalization analysis

---

## Repository structure

# vale-top-11
Business &amp; Data Analysis case study: VALE ads monetization and cannibalization check
