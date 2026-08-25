# Day 21 — Digital Privacy Dashboard

## Overview

For Day 21, I created an interactive **Digital Privacy Dashboard** based on a sample user's reported digital footprint.

The dashboard analyzes the listed digital services to estimate privacy exposure, ecosystem concentration, data collection likelihood, risk levels, and potential digital-profile insights.

> **Important:** The dashboard distinguishes between **Facts** and **Estimates**. It does not claim access to private databases or certainty about inferred personal characteristics.

---

## Sample User Dataset

### Facts

The user reported using:

- Instagram
- Snapchat
- TikTok
- YouTube
- Discord
- WhatsApp
- iMessage
- Spotify
- Roblox
- PUBG Mobile
- Amazon
- Meesho
- Google Search
- Google Pay
- Google Photos

### Dataset Rules

- All listed services are treated as **Facts**.
- Parent companies are inferred from the services.
- Behavioural, demographic, lifestyle, shopping, spending, entertainment, mobility, travel, communication, and technology-related conclusions are labeled as **Estimates**.
- No private databases are assumed to be accessible.
- When information cannot reasonably be inferred, the dashboard displays **"Not enough information provided."**

---

## Dashboard Features

The dashboard includes:

1. **Digital Footprint Score**
2. **Privacy Score**
3. **Exposure Heatmap**
4. **Company Exposure Ranking**
5. **Data Collection Matrix**
6. **Risk Radar**
7. **Digital Twin Profile**
8. **WOW Insights**
9. **Most Valuable Data Assets**
10. **Privacy Improvement Plan**
11. **Privacy Improvement Simulator**
12. **Final Verdict**

Additional metrics include:

- Total Services Used
- Number of Parent Companies
- Ecosystem Concentration Score
- Estimated Tracking Surface

---

## Score Interpretation

### Digital Footprint Score

| Score | Level |
|---|---|
| 0–30 | 🟢 Minimal |
| 31–60 | 🟡 Moderate |
| 61–80 | 🟠 Significant |
| 81–100 | 🔴 Extensive |

### Privacy Score

| Score | Level |
|---|---|
| 0–30 | 🔴 Weak |
| 31–60 | 🟠 Fair |
| 61–80 | 🟡 Good |
| 81–100 | 🟢 Strong |

---

## Key Privacy Analysis

The reported footprint contains a broad mix of:

- Social media platforms
- Messaging services
- Search services
- Entertainment platforms
- Gaming services
- E-commerce platforms
- Digital payment services
- Cloud/photo storage

This creates a potentially broad **Estimated Tracking Surface**, because different categories of services can observe different types of user activity.

The dashboard focuses on:

- Cross-platform exposure
- Parent-company concentration
- Communication exposure
- Search and browsing signals
- Shopping and transaction signals
- Entertainment preferences
- Gaming activity
- Photos and cloud-stored information

These are analytical estimates based only on the supplied dataset.

---

## Facts vs Estimates

### Facts

The following are directly provided by the dataset:

- The services listed above are used by the reported user.
- The services are treated as part of the user's digital footprint.

### Estimates

The dashboard may estimate:

- Potential interests
- Possible entertainment preferences
- Possible shopping behaviour
- Potential communication patterns
- Potential spending-related signals
- Potential technology preferences
- Possible ecosystem concentration
- Potential data-value categories

These should **not** be interpreted as confirmed personal characteristics.

---

## Privacy Recommendations

The dashboard provides privacy improvement suggestions such as:

- Review application permissions regularly.
- Reduce unnecessary location access.
- Restrict microphone and camera permissions when not required.
- Review advertising personalization settings.
- Minimize unnecessary account linking.
- Use strong and unique passwords.
- Enable multi-factor authentication.
- Review connected applications and third-party access.
- Remove unused applications and accounts.
- Regularly review cloud/photo sharing settings.

---

## Learning Outcomes

Through this task, I explored how a digital footprint can be analyzed using a structured dataset and visualized through an interactive cybersecurity dashboard.

### Key Learnings

- Digital services can create different categories of privacy exposure.
- Using many services can increase the overall digital tracking surface.
- Parent-company relationships can create ecosystem concentration.
- Data collected by platforms can have different levels of potential value.
- Digital-profile insights must be clearly separated into Facts and Estimates.
- Privacy analysis should avoid presenting inferred behaviour as certainty.
- Interactive dashboards make complex privacy information easier to understand.
- Privacy recommendations should focus on practical actions rather than fear-based assumptions.

---

## Technology Used

- HTML5
- CSS3
- JavaScript
- Interactive dashboard components
- Data visualization
- Responsive UI design

---
## Privacy Disclaimer

This project is an analytical visualization exercise.

It does not access private databases, personal accounts, browser history, device data, financial records, or any other private information.

All analysis is based exclusively on the supplied sample dataset.

Any inferred behavioural, demographic, lifestyle, shopping, spending, entertainment, mobility, travel, communication, or technology-related information is an Estimate, not a verified fact.
---
## Day 21 Goal

Build → Analyze → Visualize → Understand → Improve

The objective was to understand how a collection of everyday digital services can contribute to a user's overall digital privacy exposure and how that exposure can be communicated through an interactive cybersecurity dashboard.
