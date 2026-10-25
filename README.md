# Dashboard: Animated Gapminder Visualizations

An interactive report built with **Quarto** and **R** that uses two animated charts to show how life expectancy and wealth changed around the world between 1952 and 2007. It was created as a Data Visualization course project.

## What you'll find in the report

1. **Animation 1: countries.** Each dot is a country, placed by income per person (GDP per capita, log scale) and life expectancy, colored by continent, and animated year by year. Hover over a dot to see that country's numbers.
2. **Animation 2: continents.** An animated bar chart of average life expectancy for each continent, weighted by population so that larger countries count for more.

Each animation comes with the question it answers, a plain-language explanation of the results, and a small summary table. The report ends with lessons learned and limitations.

## View the report

GitHub shows HTML files as code, so download or clone the repository and open **`Animation_data.html`** in your browser. Keep the `Animation_data_files/` folder next to it, because the page needs it to display the charts.

## About the data

`gapminder_dataset.csv` holds 1,704 rows: 142 countries, measured every five years from 1952 to 2007. It comes from [Gapminder](https://www.gapminder.org).

| Column | Meaning |
|---|---|
| `country` | Country name |
| `continent` | Africa, Americas, Asia, Europe, or Oceania |
| `year` | Year of the observation |
| `lifeExp` | Life expectancy at birth, in years |
| `pop` | Population |
| `gdpPercap` | GDP per person (per capita) |

## Rebuild the report yourself

1. Install [R](https://www.r-project.org) and [Quarto](https://quarto.org/docs/get-started/).
2. Open a terminal in this folder and run:

   ```bash
   quarto render Animation_data.qmd
   ```

The report installs any missing R packages it needs (`plotly`, `scales`, `knitr`) the first time it runs.

## Project files

| File or folder | What it is |
|---|---|
| `Animation_data.qmd` | The source of the report: text, R code, and both animations |
| `Animation_data.html` | The finished report, ready to open in a browser |
| `Animation_data_files/` | Support files the finished report needs (charts and styling) |
| `gapminder_dataset.csv` | The data |

## Author

Made by [Muhammad Huzaifa Shafique](https://github.com/Muhammad-Huzaifa-Shafique).
