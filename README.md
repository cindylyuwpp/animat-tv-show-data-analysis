# Animated TV Shows Analysis
A data project using Python and pandas to explore animated TV shows that premiered between 1987 and 2022.

## Dataset
- Source: [Animated Television Shows Around the World (Kaggle)](https://www.kaggle.com/datasets/iamsouravbanerjee/animated-television-show)
- File used: `data/1987 - 2022.csv` (2,477 shows), included in this repo

## Questions
1. Which channels have the most shows?
2. What is the most common animation technique?
3. Did animation technique change over time?
4. How do countries differ in episodes per season and years a show ran?

## Findings
- **Channels:** Netflix has the most shows, followed by Cartoon Network.
- **Technique:** Traditional is the most common overall, but it dropped from about 95% of shows in the 1990s to about 22% in the 2020s. Flash and then CGI took over.
- **Countries:** France, Spain and Italy have the most episodes per season, and the US has the fewest. Most shows run about 1 year in every country.

## Limitations
- Shows still running have no end year, so their duration is left out.
- 699 shows have no Seasons value, so they are left out of episodes per season.
- One outlier, "3000 Whys of Blue Cat" (3,057 episodes in 1 season), distorts China's average. Next step: exclude it and use the median.

## How to Run
```bash
python3 -m venv venv
source venv/bin/activate
pip install pandas matplotlib jupyter ipykernel
jupyter notebook
```

Open `tvshows_analysis.ipynb` and choose Kernel → Restart & Run All.

## Tools
Python, pandas, matplotlib, Jupyter Notebook
