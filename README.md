<a href="https://www.linkedin.com/in/kshitija-chilbule-b98515309/" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin" alt="LinkedIn Badge" style="height: 30px; width: auto;">
</a>

# Shopping-Mall Paid Search Marketing Campaign Analysis
## Table of Contents
- [Dashboard Preview](#dashboard-preview)
- [Overview](#overview)
- [Introduction](#introduction)
- [Objectives](#objectives)
- [Data Source](#data-source)
- [Important Metrics](#important-metrics)
- [Understanding Keyword Match](#understanding-keyword-match)
- [Business Questions](#business-questions)
- [Insights](#insights)

## Dashboard Preview
## Overview
This project involves the analysis of a Paid Search Campaign for a shopping mall in the United States. The analysis covers a 5-month period in 2021, with the primary objectives of optimizing conversions, increasing profitability, and reducing costs.

## Introduction
A Paid Search Marketing Campaign is a digital advertising strategy designed to promote products or services through search engines like Google, Bing, or Yahoo. It operates on a pay-per-click (PPC) model, where advertisers bid on specific keywords to ensure their ads appear prominently in search results when users search for related terms. These campaigns are highly effective because they target potential customers based on their search intent, increasing the likelihood of conversions.

## Objectives
The primary goal of this project is to analyze the performance of a paid search campaign over the past five months and optimize it to maximize conversions and revenue while minimizing costs. The analysis focuses on achieving three key objectives:

- <b>Maximize Conversions: </b> The goal is to increase the campaign’s ability to convert potential prospects into actual customers. By analyzing conversion rates and paths from impressions, and clicks to conversions, we’ll identify campaigns from ad groups that are successful from a conversion standpoint so that they can be recommended to marketing managers for optimization.44
- <b>Increase Profits: </b> Another important goal is to increase the impact of campaigns on the profitability of shopping malls. By examining metrics such as Return on Investment (ROI) and Profit Loss, we can uncover insights about which ad groups and keywords are generating the most revenue. This information enables data-driven decisions to allocate resources effectively and invest in the areas that generate the highest returns.
- <b>Minimize Cost: </b> The third goal focuses on optimizing costs. By evaluating metrics such as Cost Per Click (CPC) and Cost Per Conversion, we aim to identify areas where costs can be reduced without sacrificing campaign performance. This approach ensures that marketing budgets are allocated efficiently, resulting in higher ROI and increased profitability.

## Data Source
The dataset is a real-world dataset comprising information from a 5-month Paid Search Campaign conducted by a U.S. shopping mall in 2021. The dataset includes detailed metrics related to ad groups, advertising performance, and campaign outcomes.
The dataset is sourced from Kaggle. [Download](https://www.kaggle.com/datasets/marceaxl82/shopping-mall-paid-search-campaign-dataset?resource=download)

## Important Metrics

### 1. Visibility and Engagement Metrics
<b>Total Impressions: </b> The total number of digital views or engagements an advertisement received, often referred to as "ad views."
```
Total Impressions = SUM('campaign_data'[Impressions])
```
<b>Total Clicks: </b> The number of clicks the advertisement received.
```
Total Clicks = SUM('campaign_data'[Clicks])
```
<b>CTR(Click Through Rate): </b> The ratio of clicks to impressions, calculated as Clicks÷Impressions, expressed as a percentage.
```
CTR = DIVIDE(SUM('Campaign Data'[Clicks]), SUM('campaign_data'[Impressions]), 0)
```
### 2. Conversion Metrics
<b>Total Conversions: </b> The number of valuable user actions (e.g., purchases, form submissions) generated from the ad.
```
Total Conversions = SUM('campaign_data'[Conversions])
```

<b>Conversion Rate: </b> The percentage of people who converted after clicking on an ad, calculated as Conversions÷Clicks.
```
Conversion Rate = DIVIDE(SUM('campaign_data'[Conversions]), SUM('campaign_data'[Clicks]), 0)
```

### 3. Cost Efficiency Metrics
<b>Total Cost: </b> The total amount the advertiser spends for a specific ad group.
```
Total Cost = SUM('campaign_data'[Cost])
```

<b>CPC(Cost Per Click): </b> The average cost incurred per click on the ad, calculated as Cost÷Clicks. A lower CPC indicates better cost efficiency.
```
CPC = DIVIDE(SUM('campaign_data'[Cost]), SUM('campaign_data'[Clicks]), 0)
```

<b>Cost Per Conversion: </b> The average cost incurred to achieve a single conversion.
```
Cost Per Conversion = DIVIDE(SUM('campaign_data'[Cost]), SUM('campaign_data'[Conversions]), 0)
```

### 4. Revenue and Profitability Metrics
<b>Total Revenue: </b> The total income generated through the advertisement.
```
Total Revenue = SUM('campaign_data'[Revenue])
```

<b>Total Sale Amount: </b> The total sales quantity derived from a specific ad group.
```
Total Sale Amount = SUM('campaign_data'[Sale Amount])
```

<b>P&L (Profit and Loss): </b> The profit is calculated as Revenue−Cost, representing the net gain or loss for a specific ad group.
```
P&L = SUM('campaign_data'[Revenue]) - SUM('campaign_data'[Cost])
```

<b>ROI (Return On Investment): </b> Measures the profitability of a campaign by comparing net profit to the total cost of the investment. 
```
ROI = DIVIDE(SUM('campaign_data'[Revenue]) - SUM('campaign_data'[Cost]), SUM('campaign_data'[Cost]), 0)
```

## Understanding Keyword Match
- <b>Exact Match: </b> Show an ad when the query has the same meaning as the keyword

- <b>1:1 Match: </b>  Show an ad when the query includes the same meaning as the keyword

- <b>Phrase Match: </b> Show an ad when the query relates to the keyword

## Business Questions

## Insights
