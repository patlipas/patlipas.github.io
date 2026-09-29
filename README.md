# Patrick Pascal — DSCI 521 Milestone 3

This repository contains my Quarto website for DSCI 521. It includes two computational blog posts analyzing Canadian fruit and vegetable consumption using Python and R.

## Software used

- Quarto 1.10.18
- uv 0.12.7
- Python 3.14
- R 4.6.1
- renv 1.2.4

## Build instructions

Clone the repository:

```bash
git clone https://github.com/patlipas/patlipas.github.io.git
cd patlipas.github.io
```

Install the Python environment:

```bash
uv sync
```

Restore the R environment:

```bash
Rscript -e 'renv::restore()'
```

Render the website:

```bash
uv run quarto render
```

The rendered website is written to:

```text
docs/
```

To open the site locally on Windows:

```bash
start docs/index.html
```

## Data

The analysis uses Statistics Canada's Canadian Indicator Framework indicator 3.1.1 on fruit and vegetable consumption.

Source:

https://sdgcif-data-canada-oddcic-donnee.github.io/3-1-1/

The CSV used by the posts is committed to this repository under:

```text
data/fruit_vegetable_canada.csv
```

Because the dataset is included in the repository, the website does not need to download the dataset from the internet during rendering.

The data are used under the Statistics Canada Open Licence.