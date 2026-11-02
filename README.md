# Strategy Unit Branding YAML

[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)

A repository containing SU branding and logos:

├── CODEOWNERS
├── LICENSE
├── logos
│   ├── logo_black.svg
│   ├── logo_black_favicon.png
│   ├── logo_black_medium.png
│   ├── logo_yellow.svg
│   └── logo_yellow_medium.png
├── README.md
├── su-brand.Rproj
├── _brand.yml
├── _SUBrand.StyleSheet.css
└── _SUBrand.toml

## For Quarto: 

See [Multiformat branding with `_brand.yml`](https://quarto.org/docs/authoring/brand.html#overview) documentation. 

## For R Shiny:
[bslib](https://rstudio.github.io/bslib/) v0.9.0+ is required to use `_brand.yml`

- For a `_brand.yml` in same directory as Shiny App add `theme = bs_theme(brand = TRUE)` to UI code to include.
- Otherwise, specify .yml file and any necessary file paths, e.g. `theme = bs_theme(brand = "folder/your_brand_file_here.yml")`

Note: logos in `_brand.yml` are not currently supported for R Shiny. Logo files that you wish to include in your Shiny App should be placed in the `www/` folder and explicitly embedded in your App.

See also [Unified theming with brand.yml](https://rstudio.github.io/bslib/articles/brand-yml/index.html#basic-usage)

## Using the logo

When using html to refer to a logo note that the alignment, size and alternative text can be coded into the html:

Yellow logo
<a href='https://www.strategyunitwm.nhs.uk/'><img src='https://raw.githubusercontent.com/The-Strategy-Unit/assets/main/logo_yellow.svg' alt="Strategy Unit" align="right" height="80" /></a>

`<a href='https://www.strategyunitwm.nhs.uk/'><img src='https://raw.githubusercontent.com/The-Strategy-Unit/assets/main/logo_yellow.svg'  alt="Strategy Unit" align="right" height="80" /></a>`

Black inverted logo
<a href='https://www.strategyunitwm.nhs.uk/'><img src='https://raw.githubusercontent.com/The-Strategy-Unit/assets/main/logo_black.svg' alt="Strategy Unit" align="right" height="80" /></a>

`<a href='https://www.strategyunitwm.nhs.uk/'><img src='https://raw.githubusercontent.com/The-Strategy-Unit/assets/main/logo_black.svg' alt="Strategy Unit" align="right" height="80" /></a>`

Alternative text does not include the word "logo" as it's not required. 
As advised by [WebAim](https://webaim.org/techniques/alttext/#logos)


## Other Info:

- general guidance website: https://posit-dev.github.io/brand-yml/

- Live Shiny App with editable `_brand.yml`: https://bslib.shinyapps.io/brand-yml/

- NHS-R Community example: https://posit-dev.github.io/brand-yml/inspiration/brand-guidelines/nhsr-community/

- StrategyUnitTheme repo: https://github.com/The-Strategy-Unit/StrategyUnitTheme

- Quarto extension: https://github.com/The-Strategy-Unit/su-theme
