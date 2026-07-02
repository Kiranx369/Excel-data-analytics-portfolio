# Excel Data Analytics Portfolio

Hi, I'm Kiran. This repo holds four Excel dashboard projects I built while learning data analytics — starting with basic data cleaning and working up to multi-table relational modeling and live API data.

Each project uses a different dataset and a different set of Excel skills, so together they show the range of what I can do: cleaning messy data, building pivot tables and slicers, designing relational data models with Power Pivot, and pulling in live data through Power Query.

---

## Project 1: Telecom Customer Churn Cleaning
**Skills:** data cleaning, deduplication, pivot tables, chart dashboards

Cleaned and analyzed a telecom customer dataset (1,277 customers) to understand churn.

**Key insights:**
- Overall churn rate is 31%, with an average customer tenure of 37 months.
- Fiber optic customers churn at **81%**, compared to **19%** for DSL — a huge gap that points to a pricing or service quality problem with fiber.
- Month-to-month contracts account for **86%** of churn, vs. just 11% for one-year and 2.5% for two-year contracts — locking customers into longer contracts (or giving them a reason to choose one) looks like the single biggest lever for reducing churn.
- Customers without tech support or online backup show noticeably higher churn — worth digging into as a retention offer.

*(Note: some "NA" entries under OnlineBackup/TechSupport are un-flagged — treated as a placeholder category for customers without internet service, not missing data.)*

---

## Project 2: HR Employee Attrition Dashboard
**Skills:** pivot tables, interactive slicers, workforce analytics

Analyzed employee attrition across departments, education fields, and job roles (79 employees) to spot retention risks.

**Key insights:**
- Overall attrition rate: 79 (out of total headcount shown), with an average job satisfaction score of 2.00/4 — on the low side.
- Attrition is highest among employees with a **Life Sciences** background (38%) and **Medical** background (36%) — far above Marketing (14%) or Technical Degree (7.7%).
- Divorced employees have noticeably higher overtime rates than married or single employees, which may be worth flagging as a wellbeing/retention factor.
- Sales and R&D account for the vast majority of business travel, which could be contributing to attrition in those departments.

---

## Project 3: Multi-Table Supply Chain Logistics Auditor
**Skills:** Power Pivot, relational data modeling (star schema), multi-table analysis

Built a relational data model connecting orders, carriers, plants, and warehouses (9,215 orders) to audit logistics performance.

**Key insights:**
- On-time shipping rate is strong overall at **96%**, with only 4% average late shipments.
- One carrier (V444_0) has a **5% late-ship rate** — 5x higher than the next carrier (V444_1 at 1%) — a clear candidate for a performance review or renegotiation.
- Plant capacity is very uneven across the network — some plants run near 1,000 units of capacity while others sit under 100, which could signal over- or under-utilized facilities.
- Product variety is heavily concentrated in a few warehouses (one warehouse alone stocks 781 product variants vs. under 30 in several others) — worth checking if that's intentional specialization or an inventory imbalance.

---

## Project 4: City of Chicago Municipal Salary & Budget Audit
**Skills:** Power Query (M code), live API data pull, text normalization

Pulled public salary data via a live API for 31,844 city employees to audit municipal spending.

**Key insights:**
- Average annual salary across all employees is **$111,550**, but the distribution is heavily skewed — most employees (20,951) fall in the $100K–150K band.
- The **Chicago Police Department** and **Chicago Fire Department** account for by far the largest share of total salary spend among all departments — expected for a city budget, but worth calling out as where the bulk of taxpayer money goes.
- The vast majority of employees (30,900) are full-time, and most are salaried rather than hourly (24,869 vs 6,975) — useful context for understanding how the city structures its workforce.

---

## What I'd improve next
- Add written insights like the ones above directly into each dashboard, not just the README.
- Standardize number formatting (currency symbols, thousands separators) across all four dashboards.
- Fix the "Attration Rate" label typo in Project 2.
