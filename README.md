# Movie Insights Analysis Project

This project performs exploratory data analysis on multiple movie-related datasets
to uncover insights on profitability, budget-revenue relationships, and the impact
of critics and audience ratings on box office performance.


# Movie Business Analysis Project

## Objective

The goal of this project is to explore multiple movie-related datasets to uncover insights about:

* Movie profitability
* The relationship between production budget and revenue
* The impact of critic and audience reviews on box office performance

This analysis supports stakeholders in making data-driven decisions in content production, marketing, and investment strategies.


## Business Understanding

**Core Business Questions:**

1. What types of movies yield the highest profits?
2. Is there a strong correlation between budget and revenue?
3. Do critic and audience reviews significantly affect a movie’s box office performance?
4. Which studios or genres perform best financially?

**Stakeholders:**

* Film production companies
* Distributors and investors
* Marketing teams
* Streaming platforms and cinemas

## Datasets Used

1. **bom.movie\_gross.csv**: Domestic and foreign gross revenue by movie and studio
2. **rt.movie\_info.csv**: Movie metadata from Rotten Tomatoes (rating, genre, box office)
3. **rt.reviews.csv**: Critic reviews and ratings
4. **tmdb.movies.csv**: Popularity, user ratings, and vote counts from TMDb
5. **tn.movie\_budgets.csv**: Production budgets and worldwide gross figures


## Data Preparation & EDA

### Step 1: Importing & Inspecting the Data

* Loaded all 5 datasets using pandas
* Inspected `.head()`, `.info()`, and `.describe()` for initial understanding

### Step 2: Cleaning

* Renamed columns for consistency
* Handled missing values (e.g., removed rows missing budget or revenue)
* Converted budget and revenue columns from strings to floats
* Removed duplicates and irrelevant columns

### Step 3: Merging Datasets

* Merged datasets on appropriate keys (e.g., `title`, `id`, or `release_date`)
* Created a master DataFrame that includes: title, budget, revenue, popularity, reviews

### Step 4: Feature Engineering

* Calculated profit as `worldwide_gross - production_budget`
* Created a profitability metric (e.g., `profit_margin = profit / budget`)
* Cleaned rating fields (critics and audience)


## Data Analysis & Visualization

### Profitability Analysis

* Bar charts of top 10 most profitable movies
* Boxplots of profitability by genre or studio
* Scatter plots: `budget vs profit`, `budget vs revenue`

### Audience & Critic Impact

* Scatter plots and correlation heatmaps for:

  * `vote_average` vs `box_office`
  * `critic_score` vs `profit`
* Bar charts showing average profits for “fresh” vs “rotten” reviews

### 🏆 Studio & Genre Performance

* Aggregated average profit by studio and genre
* Visualized using bar plots and pie charts

---

## Key Findings

1. **Budget Matters (to a point)**: Higher budgets often correlate with higher revenue—but not always with higher profits.
2. **Genre Trends**: Certain genres like animation and superhero movies are consistently profitable.
3. **Reviews Influence Success**:

   * Movies with high audience scores tend to earn more
   * Critics' reviews show a moderate impact on box office performance
4. **Studio Trends**: A few studios dominate the top spots in terms of profitability.

---

## Recommendations

1. **Invest in High-Growth Genres**: Focus production on genres like action, adventure, or animation with proven profitability.
2. **Optimize Budget Allocation**: Avoid overspending on low-return genres; prioritize efficient budget management.
3. **Leverage Review Data**: Marketing efforts should emphasize early reviews and audience buzz to drive ticket sales.
4. **Data-Informed Greenlighting**: Use historical data to guide greenlighting decisions based on similar successful films.

## Tools & Technologies

* **Languages**: Python (Pandas, NumPy, Matplotlib, Seaborn)
* **IDE**: VS Code
* **Database**: SQLite (for merging and querying large datasets)
* **Version Control**: Git + GitHub

---

## Future Work

* Integrate streaming data for post-theatrical revenue analysis
* Apply machine learning models to predict profitability
* Dashboard creation using Plotly or Power BI

