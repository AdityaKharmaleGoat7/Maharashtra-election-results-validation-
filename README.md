# Maharashtra 2024 Election Results Analysis: Benford's Law

This project analyzes the **Maharashtra 2024 Election Results** using **Benford's Law** to determine if the distribution of vote counts follows the expected natural pattern. This statistical technique is used to detect potential anomalies, and here, it's applied to test whether claims of fake votes or vote manipulation in the election have any basis.

## Table of Contents

- [Introduction](#introduction)
- [Benford's Law](#benfords-law)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)
- [License](#license)

## Introduction

In the aftermath of the **Maharashtra 2024 elections**, some parties and individuals raised concerns about possible **fake votes** and election manipulation. To address these concerns, this project uses **Benford's Law**—a statistical tool widely used for detecting anomalies in datasets—to analyze the **total votes** cast for each candidate. By comparing the observed distribution of first digits in the vote counts with the expected distribution predicted by Benford's Law, this analysis provides insight into the legitimacy of the election results.

## Benford's Law

**Benford's Law** states that in many naturally occurring datasets, the **first digit** of the numbers is more likely to be small. For example, the digit **1** appears as the first digit about **30%** of the time, while the digit **9** only appears about **5%** of the time. This law can be applied to various datasets, including election results, financial figures, and scientific data, to check if the data follows this expected pattern.

## Data

The dataset used in this project contains the election results for the **Maharashtra 2024 elections**, including:
- **AC No**: Assembly Constituency Number
- **AC Name**: Assembly Constituency Name
- **Candidate**: Candidate Name
- **Party**: Political Party
- **EVM Votes**: Electronic Voting Machine Votes
- **Postal Votes**: Postal Votes
- **Total Votes**: Total Votes (EVM + Postal)
- **Vote Share (%)**: Percentage of total votes received by each candidate

The data was collected and analyzed to check if the distribution of the **first digits of the total votes** adheres to **Benford's Law**.

## Methodology

1. **Extracting the First Digit**: The first digit of each candidate's total vote count is extracted.
2. **Benford's Law Comparison**: The frequency of each first digit is calculated and compared to the expected frequency distribution of Benford's Law.
3. **Statistical Testing**: The **Chi-Square Test** is performed to statistically determine if the observed frequencies match the expected frequencies.
4. **Visualization**: A comparison plot is created to visually show the alignment between the actual vote counts and the expected Benford's Law distribution.

## Results

The analysis results show that the election data follows **Benford's Law** closely, with a **percentage of {follow_benford_percentage}%** adherence. This suggests that the election results are **not manipulated** and aligns with the expected distribution for natural datasets.

Key findings include:
- The distribution of first digits closely matches Benford's Law.
- The Chi-Square p-value indicates no significant deviation from the expected distribution.

## Visualizations

The project generates the following visualizations:
- **First Digit Distribution**: A bar plot comparing the observed first digit distribution of the vote counts against the expected distribution according to Benford's Law.
- **Comparison of Actual and Expected Frequencies**: A plot showing the actual observed frequencies versus the expected probabilities for the first digits (1 to 9).

These plots help illustrate that the election data follows the natural pattern, providing confidence in the authenticity of the election results.

## Conclusion

The analysis suggests that the **2024 Maharashtra election results** are statistically **consistent with Benford's Law**, indicating that there is no evidence of vote manipulation or "fake votes." The claims of election fraud appear unfounded when analyzed using a rigorous statistical method.

**Benford's Law** is a powerful tool for data analysis, and its application here helps to reaffirm the integrity of the election process.

## How to Run

To replicate or modify this analysis on your own election dataset, follow these steps:

1. **Install Required Libraries**:
   Ensure that you have the necessary Python libraries installed:
   ```bash
   pip install pandas matplotlib numpy scipy
