# Install package

## 1. Install Quarto (skip if installed)

```         
install.packages("quarto")
```

## 2. Install r-package "tinytex" (skip if installed)

```         
install.packages("tinytex")
```

## 3. Install TinyTex via r-package (skip if installed)

```
tinytex::install_tinytex()
```

## 4. Create new folder for you bachelor project

## 5. Change RStudio working directory to new folder

## 6. Get template from Github via quarto

```         
quarto::quarto_use_template("OffByOne37/bachelor_template")
```

## 7. Render index.qmd (If first itme rendering with TinyTex then it will take quiet some time)

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
