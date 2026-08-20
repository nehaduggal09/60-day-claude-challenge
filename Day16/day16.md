# Day 16 — Custom Skill: Stock Fundamental Research

## 📌 Task Overview

For Day 16 of the 60 Days Claude AI Challenge, I created a custom Claude Skill named **`stock-fundamental-research`**.

The purpose of this skill is to analyze Indian and global listed companies using fundamental research, financial statements, valuation, business quality, competitive advantages, ownership trends, risks, and growth prospects.

The skill is designed to generate **evidence-based, investor-friendly research reports** without providing direct Buy/Sell/Hold recommendations or personalized investment advice.

---

## 🎯 Skill Name

`stock-fundamental-research`

### Description

Analyze Indian and global listed companies using fundamentals, financial statements, business quality, competitive advantages, valuation, risks, and growth prospects. Generate evidence-based research reports and investor-friendly summaries. Never provide direct buy, sell, or hold recommendations.

---

## 🔍 What the Skill Can Do

The custom skill supports multiple research modes:

### 1. Quick Take
Provides a short fundamental overview of a single stock, including:

- Company overview
- Current Market Price (CMP)
- Market Capitalization
- P/E and valuation view
- Debt-to-Equity
- ROE and ROCE
- Growth trend
- Key strengths
- Watch-points
- Fundamental Quality
- Stock price chart

### 2. Deep Dive
Provides a detailed fundamental research report covering:

- Snapshot
- Valuation
- Growth
- Financial Health
- Returns
- Peer Comparison
- Ownership
- Overall View
- Strengths and risks
- Data confidence
- Price chart

### 3. Compare
Allows comparison of two stocks using metrics such as:

- CMP
- Market Cap
- P/E
- P/B
- EV/EBITDA
- Revenue CAGR
- Profit CAGR
- EBITDA Margin
- ROE
- ROCE
- Debt-to-Equity
- Promoter Holding
- Pledging
- Dividend

The comparison remains neutral and does not declare an investment winner.

### 4. Pros & Cons
Identifies evidence-backed:

- Strengths
- Risks
- Business advantages
- Financial concerns
- Balanced fundamental summary

### 5. Portfolio Fit
Analyzes a stock in the context of an existing portfolio by looking at:

- Concentration
- Sector overlap
- What the stock adds
- What it duplicates
- Fundamental snapshot
- Neutral portfolio-fit discussion

---

## 📊 Fundamental Metrics Covered

The skill researches:

- CMP
- Market Cap
- Face Value
- 52-Week High/Low
- P/E
- P/B
- EV/EBITDA
- Revenue CAGR
- Profit CAGR
- EPS CAGR
- EBITDA Margin
- Net Profit Margin
- EPS for the last 8 quarters
- Free Cash Flow
- Debt-to-Equity
- Interest Coverage
- Current Ratio
- ROE
- ROCE
- Dividend history
- Dividend payout
- Promoter holding
- Promoter pledging
- FII/DII trends
- Peer fundamentals
- Business quality
- Competitive advantages
- Market share
- Pricing power
- Switching costs
- Management quality
- Governance
- Sector trends
- Latest earnings commentary
- Relevant company news

---

## 📈 Interpretation Framework

The skill uses predefined fundamental interpretation rules.

### Valuation

- **Cheap:** Below sector valuation and historical valuation
- **Fair:** Within approximately 10%
- **Expensive:** Above sector and historical valuation

### Debt-to-Equity

- **< 1:** Safe
- **1–2:** Moderate
- **> 2:** Leveraged

### Interest Coverage

- **> 3:** Healthy
- **1.5–3:** Watch
- **< 1.5:** Risk

### Current Ratio

- **> 1.5:** Comfortable
- **1–1.5:** Watch
- **< 1:** Risk

### Free Cash Flow

- Positive & growing → **Strong**
- Positive & stable → **Stable**
- Negative → **Concern**

### ROE / ROCE

- **> 15%:** Good
- **10–15%:** Average
- **< 10%:** Weak

### Growth

Growth can be classified as:

- Accelerating
- Steady
- Slowing
- Declining

---

## 🌐 Data & Source Priority

The skill is designed to prioritize live and reliable information.

Source priority:

1. Screener
2. Tickertape
3. Moneycontrol
4. NSE
5. BSE
6. Annual Reports
7. Earnings Calls

Important figures should be cross-checked using at least two sources.

If live information cannot be retrieved, the report should clearly state:

> Live data couldn't be fetched; figures may be outdated.

The skill must never fabricate unavailable financial data.

---

## 🛡️ Responsible Research Rules

The skill follows these important rules:

- No Buy recommendation
- No Sell recommendation
- No Hold recommendation
- No target price
- No personalized investment advice
- No fabricated figures
- Key figures must include sources
- Historical trends should not be presented as guaranteed future outcomes
- Jargon should be explained in simple English
- Data limitations should be clearly disclosed

---

## 📉 Charts & Analysis

The skill also includes visual analysis such as:

- Stock price chart
- Valuation comparison
- Ownership trends
- Fundamental metric comparisons
- Peer comparisons
- Other relevant stock-related charts

Charts are used to make the research easier to understand.

---

## 🧪 Testing

The skill can be tested using Indian listed companies such as:

- TCS
- Infosys
- Reliance Industries
- HDFC Bank
- Tata Motors

Example prompts:

``` text
Analyze TCS using the stock-fundamental-research skill.
```
