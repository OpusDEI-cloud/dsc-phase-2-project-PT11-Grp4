# 🎬 Phase 2 Group 4 Project – Movie Data Analysis

## 📘 Overview
This project notebook is a comprehensive analysis performed by **Group 4** as part of **Phase 2**. The objective is to help a company planning to start a movie studio understand what types of films are successful at the box office. The analysis includes data cleaning, exploratory data analysis (EDA), modeling, and evaluation using multiple industry data sources.

## 🎯 Business Understanding
**Key Business Question:**  
*What kinds of movies should a new studio produce to maximize financial success?*

### Stakeholders:
- Studio executives and investors
- Marketing strategists
- Creative development teams

### Objectives:
- Identify high-performing genres
- Understand budget-to-revenue relationships
- Evaluate impact of critical and audience reviews

## 📂 Contents
- **Data Preprocessing**: Integration and cleaning of movie datasets from multiple sources  
- **Exploratory Data Analysis (EDA)**: Trends, genres, revenue, ratings, and other insights  
- **Modeling**: Data-driven analysis using machine learning and regression models  
- **Model Evaluation**: Performance metrics and validation to ensure relevance

## 📈 Data Understanding and Analysis
### Source of Data:
The datasets were compiled from:
- Box Office Mojo
- IMDB
- Rotten Tomatoes
- TheMovieDB
- The Numbers

### Description of Data:
- **Budget**: Estimated production costs
- **Revenue**: Worldwide gross income
- **Genres**: Categorical tags for movie types
- **Ratings**: IMDB and Rotten Tomatoes scores
- **Metadata**: Release dates, production companies, etc.

### Visualizations:
1. **Genre vs. Average Profitability**  
   ![Genre Profitability](visualizations/genre_profitability.png)

2. **Production Budget vs. Revenue**  
   ![Budget vs Revenue](visualizations/budget_vs_revenue.png)

3. **Review Scores vs. Revenue**  
   ![Review Score Impact](visualizations/review_score_impact.png)

## 🧠 Key Insights
- Films with higher ratings on **Rotten Tomatoes** and **IMDB** tend to perform better at the box office.
- **Action** and **Adventure** films usually yield higher revenues.
- There is a positive correlation between **budget** and **revenue**, but with diminishing returns at high budget levels.
- Combining multiple data sources enhances prediction reliability and decision-making accuracy.

## 📊 Tools and Libraries
- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  
- Jupyter Notebook  

## 📁 How to Use
Clone the repository and run the analysis:

```bash
git clone https://github.com/OpusDEI-cloud/dsc-phase-2-project-PT11-Grp4.git
cd dsc-phase-2-project-PT11-Grp4
code .
```

Open the notebook and run it in **Jupyter Notebook** or **VS Code**.

## ✅ Conclusion
This analysis offers key strategic insights for new movie studios:
- Prioritize high-performing genres like Action and Adventure.
- Focus on balanced budgeting to maximize ROI.
- Use review metrics as an early indicator of potential financial success.

## 🤝 Contributors
- Ragot Raphael  
- Deborah Omondi  
- Kelvin Shilisia  
- George Kariuki  
- Mohamed Sheikh  
- Jennipher Anyango  

## 📜 License
This project is open source with no particular license.
