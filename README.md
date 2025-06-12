# Movie Correlation 
This Repository contains files that have been used for my portfolio projects. Feel free to check them out, and please reach out if you have any questions and/or inquiries.

**Project Overview**
This analysis explored a dataset of hundreds of movies—covering attributes like release year, budget, gross earnings, ratings, and more—to uncover patterns in budget allocation, box‑office performance, and the relationships between various film features.

**Objectives**
- Clean and preprocess the raw movie dataset.
- Visualize the relationship between production budgets and gross revenue.
- Compute and interpret correlations among numeric and categorical features.
- Identify which factors most strongly predict box‑office success.

**Key Steps & Techniques**
- Environment Setup & Data Ingestion
- Imported pandas, numpy, matplotlib, and seaborn.
- Configured plot style (ggplot) and default figure size.
- Loaded the CSV file into a DataFrame for analysis.

**Data Cleaning & Type Conversion**
- Missing Data: Computed percent of nulls per column to assess completeness.
- Numeric Conversion: Coerced non‑numeric entries in budget and gross to zero and cast to int for accurate math.
- Date Extraction: Created yearcorrect by slicing the year from the released string.
- Negative Values: Transformed any negative gross figures to their absolute values.
- Duplicates: Inspected and dropped duplicate company names to avoid skewed group analyses.
- Exploratory Data Visualization
- Scatter Plot: Plotted budget vs. gross to see raw dispersion of production spend against box‑office returns.
- Regression Plot: Added a Seaborn regplot overlay (red dots, blue line) to highlight the linear trend between budget and revenue.

**Correlation Analysis**
- Numeric Correlations: Computed a Pearson correlation matrix among all numeric features and displayed it via a heatmap.
- Categorical Encoding: Converted string columns (e.g. genre, director, company) into integer codes to incorporate them into the correlation matrix.
- Re‑evaluation: Re‑computed and visualized the updated heatmap to include encoded categorical features.
- Strongest Relationships: Unstacked, sorted, and filtered correlation pairs to identify the highest correlation values (>0.5), revealing that budget and votes are the strongest predictors of gross.

**Outcome**
- Demonstrated a clear positive correlation between production budget and box‑office gross.
- Identified key factors—particularly budget and audience votes—that align most closely with financial success.
- Produced clean, well‑documented code and visual assets suitable for presentation or integration into a dashboard.

**What I Learned**
- Best practices for handling missing and malformed data in pandas.
- Techniques for extracting and engineering new features (e.g., parsing date strings).
- How to layer Matplotlib and Seaborn visualizations to tell a more compelling story.
- Strategies for encoding and analyzing categorical data alongside numeric features.
