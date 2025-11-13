# ibm-project
# Netflix Exploratory Data Analysis (EDA)

## Project Overview
This project performs an Exploratory Data Analysis (EDA) on the Netflix Titles dataset (`netflix_titles.csv`) to uncover insights about the streaming platform’s catalogue. The dataset includes information such as title type (Movie or TV Show), release year, genre(s), country of origin, cast, director, date added, rating, and duration.  
Using Python (pandas, numpy) for data manipulation, matplotlib & seaborn for visualisation, and Streamlit for dashboard deployment, the project flows through data cleaning, feature engineering, insightful visualisations and interactive deployment.

## Motivation
With the streaming market rapidly growing, understanding content trends is vital. This analysis helps answer questions like:
- What is the distribution of Movies vs TV Shows on Netflix?
- Which genres and countries dominate the catalogue?
- How has content addition evolved over time?
- What are patterns in content ratings, durations, and contributors (actors/directors)?

## Dataset
- **Filename**: `netflix_titles.csv`  
- **Source**: https://www.kaggle.com/datasets/shivamb/netflix-shows/data
- **Main fields**: `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in` (genres)  

## Implementation Details
- Loaded and inspected the data using pandas; removed duplicate entries and filled missing values for key columns (e.g., `country`, `rating`, `date_added`).  
- Converted `date_added` to datetime, extracted the `year_added`, and parsed `duration` to separate movie minutes vs TV show seasons.  
- Split multi-valued string columns (genres, cast, country) using `.split(', ')` and `.explode()` for frequency analysis.  
- Visualised distributions: Movies vs TV Shows; Top genres; Top countries; Content added per year; Rating distribution; Duration and seasons; Top directors and actors.  
- Deployed a Streamlit dashboard where users can upload the dataset, view metrics, and explore plots interactively.

## Tools & Technologies
- Python 3.11.9 
- pandas, numpy  
- matplotlib, seaborn  
- Streamlit  
- Jupyter Notebook (initial exploration)  
- Dataset: `netflix_titles.csv`

## How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/NikhilArora06/EDA-on-netflix-dataset
2. Install Dependencies
pip install -r requirements.txt
3. To launch Streamlit
   streamlit run app2.py  



