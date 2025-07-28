# A/B Testing in Two Different Business Contexts

This project contains two distinct projects:

1. Fast Food Marketing Analysis
2. Video Game A/B Testing

Both projects are data-driven analyses designed to perform A/B testing of strategies and user behavior.

## Libraries needed to execute the code

As can be seen in the accompanying requirements.txt file, this code uses a variety of different libraries. These can be seen there. In running the code, ensure that you have all these downloaded and installed.


## Fast Food Marketing Analysis

### Objective

Analyze sales data to assess the effectiveness of different promotional strategies in the fast food sector.

### Methodology

Data Collection: Sales data was gathered from multiple vendors, and was already collected by an external source, and collected here for this analysis via kaggle (https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test)

#### Statistical Analysis:

- ANOVA Test: Used to determine if there are significant differences between promotional strategies.
- Tukeys Pair-Wise significance test: Used to test for differences between groups, after the ANOVA indicates significance.

Visualizations: 
- Histograms
- Q-Q plots
- Bar Charts

### Key Insights

Identified sales trends linked to different promotional strategies. Specifically, promotion strategy 2 and 3 were indicated as being significantly better than strategy 1. However, based on the statistical tests, further indications of which of these two were the most successful could not be supported. A further analysis through Looker however, showed that there is perhaps some sparse indications for strategy 3 showing slightly better behavior than strategy 2 - though this, as mentioned, holds no statistical support. The Looker report can be observed here: https://lookerstudio.google.com/u/0/reporting/0b087836-5d77-4f70-9c38-99f09426cf8c/page/3f9EF/edit

## Video Game A/B Testing

### Objective

Evaluate the impact of two different game versions (gate_30 and gate_40) on player engagement, measured by the number of rounds played.

### Methodology

Data Collection: Game session data collected for 40,000+ users per version, and was already collected by an external source, and collected here for this analysis via kaggle (https://www.kaggle.com/datasets/mursideyarkin/mobile-games-ab-testing-cookie-cats)

#### Statistical Analysis:

- Kolmogorov-Smirnov Test: Used to assess data normality.
- Mann-Whitney U Test: Applied due to non-normal distributions and large sample sizes.

Visualizations:
- Histograms to visualize distribution shapes.
- Q-Q plots for further normality assessment.

### Key Insights

Ultimately, no significant difference between the two different types of game mode in influencing the amount of games a player plays could be witnessed.