### **🏛 2016 U.S. Presidential Election Poll Data**
#### 📊 **Overview**
This repository includes polling data from **FiveThirtyEight** and the **USC Dornsife/Los Angeles Times Daybreak Poll** for the 2016 U.S. Presidential Election. These datasets track **Trump vs. Clinton polling trends**, voter demographics, and predicted election outcomes.

---

## **📚 Poll Data Files**
The dataset consists of two primary sources:

1. **FiveThirtyEight Polls** (`president_general_polls_2016.csv`)
   - Aggregated polling data from various pollsters.
   - Provides **Trump vs. Clinton** adjusted polling percentages over time.
   - Includes **pollster name, sample size, methodology, and margin of error**.

2. **USC Dornsife/LA Times Daybreak Polls** (`popvote_votergroups.csv`)
   - Uses a **7-day rolling window** methodology.
   - Tracks voting intentions and predicted outcomes based on different voter demographics.
   - Data available for **popular vote share, win probability, and voter intentions**.

---

## **📂 USC Daybreak Poll Data Structure**
Each file in the **USC Dornsife/LA Times dataset** is a **tab-delimited text file** with the following structure:

| **Column** | **Description** |
|------------|---------------|
| `date` | The last day of a **7-day rolling window** (e.g., "07/10/2016" includes 07/04-07/10 data) |
| `N` | Sample size for that day |
| `Trump (%)` | Predicted percentage of votes for Donald Trump |
| `Clinton (%)` | Predicted percentage of votes for Hillary Clinton |
| `sediff` | Standard error of the Trump-Clinton vote difference |
| `Lo` | Lower uncertainty boundary (gray area in the poll graphs) |
| `Up` | Upper uncertainty boundary (gray area in the poll graphs) |

---

## **📀 Breakdown of USC Poll Files**
USC Daybreak polls also contain breakdowns based on **demographics**.

| **File Name** | **Breakdown Variable** |
|--------------|----------------------|
| `win.csv` | Overall win probability prediction |
| `pop.csv` | Popular vote share predictions |
| `int.csv` | Voter intention breakdown |
| `pop_sex_0.csv` | Female voter polling results |
| `pop_sex_1.csv` | Male voter polling results |
| `pop_rac_1.csv` | White voter polling results |
| `pop_rac_2.csv` | African-American voter polling results |
| `pop_rac_4.csv` | Hispanic voter polling results |
| `pop_age_1.csv` | 18-34 age group results |
| `pop_age_2.csv` | 35-64 age group results |
| `pop_age_3.csv` | 65+ age group results |
| `pop_edu_1.csv` | High school or less education level |
| `pop_edu_2.csv` | Some college or associate's degree |
| `pop_edu_3.csv` | Bachelor's degree or more |

🟢 Files of the format **`type_variable_category.csv`** represent a **specific subgroup** of voters.

---

## **📈 Key Insights from the Polls**
1. **Polling Methodology**
   - FiveThirtyEight aggregates multiple poll results, adjusting for **bias and accuracy**.
   - USC Daybreak uses a **rolling 7-day average** to smooth polling trends.

2. **Voter Demographic Trends**
   - The **race breakdown** helps identify differences in Trump vs. Clinton support.
   - The **education and income breakdowns** provide insight into socioeconomic voting patterns.

3. **Margin of Error & Uncertainty**
   - The **Lo & Up values** indicate polling uncertainty (gray shaded area in visualizations).
   - The **standard error (sediff)** shows the confidence in the Trump-Clinton difference.

---

## **📊 How to Use This Data**
- **Track overall polling trends** from **July to November 2016**.
- **Analyze voting patterns** across different **demographics** (race, gender, income, education).
- **Compare poll predictions** with **actual election results**.

---

## **📚 References**
- [FiveThirtyEight Polling Data](https://projects.fivethirtyeight.com/polls/)
- [USC Dornsife / LA Times Daybreak Poll](https://cesrusc.org/election/)

---

### 🔍 **Next Steps**
- **Compare polling trends with campaign events & speeches.**
- **Analyze sentiment in speeches alongside poll fluctuations.**
- **Visualize demographic shifts over time.**

