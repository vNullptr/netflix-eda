# Netflix Content — Exploratory Data Analysis

Exploratory data analysis of the Netflix titles catalogue (~8,800 titles), built with **pandas**, **NumPy**, **Matplotlib**, and **Seaborn**. The goal is to clean a messy real-world dataset and answer a set of concrete questions about how Netflix's catalogue is composed and how it has changed over time.

## Questions explored

- What is the proportion of Movies vs TV Shows on Netflix?
- How has the Movie/TV-Show balance shifted year over year?
- Which countries contribute the most content?

## What the notebook covers

- **Data inspection** — shape, dtypes, uniqueness, duplicate checks
- **Missing-value handling** — quantifying nulls per column (`director`, `cast`, `country` are the worst offenders), visualising them with a heatmap, then dropping/imputing depending on the column
- **Feature engineering** — parsing `date_added` into a datetime and deriving `year_added`
- **Visual analysis** — count plots, line plots, and grouped proportions to surface trends

## Key findings

- Netflix's catalogue is **predominantly Movies**.
- **No TV Shows appear in the early years (2008–2013)**; TV content ramps up later as Netflix pivots toward original series.
- The majority of content originates from the **US, India, and the UK**.

## Tech stack

`Python` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Jupyter`

## Running it

```bash
git clone https://github.com/vNullptr/netflix-eda.git
cd netflix-eda
pip install pandas numpy matplotlib seaborn jupyter
```

Download the dataset from [Kaggle — Netflix Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows) and place the CSV inside a `data/` folder, then open `notebook.ipynb`.

## Dataset

[Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows) (Kaggle, public).