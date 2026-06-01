# Exploratory Data Analysis — Movies Dataset

**Author:** Anoushka Gupta

---

## Overview

An exploratory analysis of a movies dataset (~45,000 films) sourced from The Movie Database (TMDB). The goal was to uncover patterns in financial performance, audience reception, and the people behind the films — directors, actors, and franchises.

---

## Dataset

The dataset contains one row per movie with features including budget, revenue, genres, cast, director, production companies, release date, ratings, and popularity scores.

Key data quality note: a large share of entries have $0 for budget and revenue, likely representing missing data rather than true zeros. These were accounted for when computing ROI and profitability metrics.

---

## Questions Explored

- Which movies generated the highest revenue, profit, and return on investment?
- Are franchise films more successful than standalone films?
- Which directors and actors are associated with the highest revenue and ratings?
- What words dominate movie titles and taglines?

---

## Key Findings

**Financial performance**
High budget does not guarantee high profit. ROI was filtered to movies with a budget of at least $10M to avoid misleading results from micro-budget outliers.

**Franchises vs. standalone films**
Franchise films earn significantly more revenue on average and carry larger budgets but their median ROI and average audience ratings are comparable to standalone films. Studios spend more without a guaranteed improvement in audience reception.

**Directors**

**Most active directors (by number of films)** : 
The most prolific directors in the dataset skew heavily toward horror and genre filmmaking : Paul W.S. Anderson, James Wan, and Wes Craven lead on total revenue, driven by franchises like Resident Evil, The Conjuring, and Scream respectively. Spielberg appears at 7th despite having far fewer films, which speaks to his consistent box office draw.

**Highest rated directors (filtered to ≥10 films and ≥10,000 total votes)**
Hayao Miyazaki leads with a mean rating of 7.70 across 14 films : the highest in the table despite having the smallest filmography among those listed. Christopher Nolan follows at 7.62 across 11 films with the highest total vote count of any director (67,344), suggesting both critical and popular appeal. Quentin Tarantino, Wes Anderson, and David Fincher round out the top five. Notably, Martin Scorsese has the largest filmography in this filtered group at 39 films, yet still maintains a 7.22 mean — a sign of remarkable consistency across a long career.

**Actors**
Total revenue is a misleading metric for actor success — Stan Lee and Samuel L. Jackson rank highest largely due to Marvel Cinematic Universe cameos and appearances, not individual performance quality. Filtering to actors with 30+ films and ranking by mean rating surfaces more meaningful results, with Toshirō Mifune leading — a Japanese cinema icon known for his collaborations with Akira Kurosawa.

**Word clouds**
Words like "love", "man", "girl", "night", and "world" dominate movie titles and taglines, reflecting recurring Hollywood themes around identity, conflict, and romance.

---

## Tools Used

- Python
- pandas
- matplotlib
- NumPy
- WordCloud

---
