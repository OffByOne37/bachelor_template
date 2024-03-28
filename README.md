# Install package

## 1. Install Quarto (skip if installed)

```         
install.packages("quarto")
```

## 2. Install "tinytex"

```         
install.packages("tinytex")
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

### Problem with package "gt"

Chapter "03-chapter-2.qmd" contains the following code snippet:

```{r tbl-1}
#| tbl-cap: "This is Table 1, which contains the `mtcars` dataset"
library(gt)
mtcars |>
    head() |>
    gt()
```

If you need package "gt" it is recommended to install it via the following command:

```         
install.packages("gt")
```

otherwise you can also delete this code snippet and it won't cause problems when rendering.
