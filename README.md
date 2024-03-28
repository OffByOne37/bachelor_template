# Install package

## 1. Install Quarto (skip if installed)

```         
install.packages("quarto")
```

## 2. Install "tidyverse"

```         
install.packages("tidyverse")
```

## 3. Create new folder for you bachelor project

## 4. Change RStudio working directory to new folder

## 5. Get template from Github via quarto

```         
quarto::quarto_use_template("OffByOne37/bachelor_template")
```

## 6. Render index.qmd

```         
click render button in RStudio
```

or use

```         
quarto::quarto_render(".")
```
