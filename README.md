# FIFA Players Insights ⚽

An exploratory data analysis of ~18,000 FIFA player records — digging into what makes a player rated, valuable, and unique across positions, ages, and nationalities. Built as a hands-on practice project combining **pandas**, **matplotlib**, **seaborn**, and **Plotly/Cufflinks** for both static and interactive visualizations.

## 📊 What's Inside

The notebook (`fifa.ipynb`) walks through a full analysis pipeline:

1. **Load & Inspect** — dataset shape, dtypes, null/duplicate checks
2. **Data Cleaning** — handling nulls in national team fields and contract values
3. **Shape of the Squad** — rating, age, and value distributions; foot preference; most-played positions
4. **Does Age Predict Greatness?** — peak performance years, young high-potential prospects
5. **What Makes a Player Valuable?** — rating vs. market value, multi-attribute pairplot
6. **Anatomy of a Position** — which skills correlate, and how attackers/midfielders/defenders/goalkeepers compare
7. **Who Gets Picked?** — national team vs. club-only players, top-performing nationalities
8. **What Drives Value?** — full correlation heatmap across all 40+ numeric attributes
9. **Room for Growth** — hidden gems (high potential, low current rating) vs. players who've already peaked
10. **Does Body Size Matter?** — height/weight vs. physical attributes, build by position, top speed demons

## 🛠️ Tech Stack

- **pandas / numpy** — data cleaning and manipulation
- **matplotlib / seaborn** — statistical visualizations
- **Plotly Express / Cufflinks** — interactive charts and dashboards
- **statsmodels** — regression trendlines (OLS, LOWESS)
- **kaleido** — static image export for GitHub-friendly notebook rendering

## 📁 Dataset

`fifa_players.csv` — ~18,000 player records with 50+ attributes including ratings, potential, market value, wages, physical stats, and detailed skill attributes (finishing, dribbling, tackling, etc.).

## 🚀 Running Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/saadnaeem463/Fifa-Players-Analytics.git
   cd Fifa-Players-Analytics
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook fifa.ipynb
   ```

> **Note:** Plotly charts in this notebook render as static PNGs (via `kaleido`) so they display correctly on GitHub. If you want full interactivity (hover, zoom), remove the `renderer="png"` argument from `fig.show()` calls and re-run locally.

