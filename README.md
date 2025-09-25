# Financial Data Analytcs Group Project
This is a project repository for our group project for our Financial Data Analytics I course. Current project timeline & deliverables:

- **Week 11**: *Project Proposal Due*
  - A one-page document outlining your chosen dataset, research questions, and initial plan.
- **Week 14**: *Final Presentation*
  - Live in-class presentations. Submit presentation slides (.pptx or PDF) before class.
- **Finals Week**: *Final Submission Due*
  - Final code, written report (grad students), and peer evaluation forms due.
 
---
 
## Project Phases

### Phase I: Dataset Selection & Proposal (Due End of Week 11)
- Research Questions: Propose 2-3 specific questions you aim to answer. These questions should guide your analysis.
- Initial Plan: Briefly outline the analytical steps you plan to take (e.g., "We will calculate daily returns, compute rolling volatility, and visualize the comparison with a line plot.")

### Phase II: Analysis & Visualization (Week 12 & 13)
1. Data Acquisition: Use a library to fetch your chosen data into a Pandas DataFrame.
2. Data Cleaning & Wrangling:
  - Inspect the data for missing values (NaN) and decide on a strategy to handle them (e.g., fill, drop).
  - Ensure data types are correct (e.g., dates are datetime objects).
  - Create new columns as needed for your analysis (e.g., daily returns, moving averages).
3. Descriptive Statistical Analysis:
  - Use Pandas and NumPy to calculate key summary statistics (e.g., mean, median, standard deviation, variance, correlation).
  - For time-series data, consider calculations like rolling averages, volatility, or beta.
  - Use groupby() to aggregate data and uncover insights (e.g., average returns by year or by company).
4. Data Visualization:
  - Create at least three distinct and meaningful visualizations that help answer your research questions.
  - Each plot must be clearly labeled with a title, axis labels, and a legend if necessary.
  - Choose the right type of plot for your data (e.g., line plot for time-series, histogram for distribution, scatter plot for correlation).

### Phase III: Presentation & Reporting
- Length: Maximum 20 minutes, followed by 5 minutes for Q&A.
- Format: A professional slide deck.
- Content:
  1. Introduction: Introduce your group, dataset, and research questions.
  2. Methodology: Briefly explain your data cleaning and analysis process.
  3. Analysis & Findings: Present your key statistical findings.
  4. Visualizations: Showcase your plots and explain what insights they reveal.
  5. Conclusion: Summarize your findings and answer your initial research questions. What are the key takeaways?
  6. Challenges & Future Work: Briefly discuss any challenges you faced and how you might extend this analysis

---

## Dataset Requirements 
- Source: Data must be acquired programmatically using a Python library such as yfinance, pandas-
datareader, or another approved financial data API. Manually downloading a CSV is not permitted.
- Complexity: The dataset should be complex enough to require meaningful cleaning and analysis. A single stock's price history is likely too simple.
- Scope: Consider comparing multiple assets (e.g., stocks, ETFs), analyzing a portfolio, or examining
economic indicators alongside market data

---

## Peer Evlations
Peer evaluations are a requirement at the end of this project. 

