# Learning the Tidyverse: A Comprehensive Guide

The **Tidyverse** is a collection of R packages designed to make data science easier. This guide covers the core and supporting packages in Tidyverse, providing key functions and learning steps for each.

## 📌 Core Tidyverse Packages

### 1. ggplot2 (Data Visualization)
**Key Functions:**
- `ggplot() + geom_*()` – Create plots with layers
- `aes()` – Aesthetics mapping
- `facet_wrap()` – Faceting for small multiples
- `theme_*()` – Customize themes

**Learn:**
- Basic scatter, bar, line, histogram plots
- Customizing aesthetics (colors, themes, labels)
- Multi-faceted plots and annotations

---
### 2. dplyr (Data Manipulation)
**Key Functions:**
- `filter()` – Select rows based on conditions
- `select()` – Pick columns
- `mutate()` – Create new variables
- `summarise()` – Aggregate data
- `group_by()` – Grouping for summarization

**Learn:**
- Data filtering, transformations, and summarization
- Chaining operations with `%>%`
- Working with grouped data

---
### 3. tidyr (Data Tidying)
**Key Functions:**
- `pivot_longer()` – Convert wide to long format
- `pivot_wider()` – Convert long to wide format
- `separate()` – Split column into multiple columns
- `unite()` – Combine multiple columns into one

**Learn:**
- Converting messy data into structured format
- Handling missing values
- Spreading and gathering data

---
### 4. readr (Data Import)
**Key Functions:**
- `read_csv()` – Read CSV files
- `read_tsv()` – Read tab-separated values
- `read_delim()` – Read delimited files
- `write_csv()` – Write data to CSV

**Learn:**
- Efficient data import and export
- Parsing different file types
- Handling large datasets

---
### 5. purrr (Functional Programming)
**Key Functions:**
- `map()` – Apply function to list/vector
- `map_df()` – Return data frames
- `map_dbl()`, `map_chr()` – Return numeric/character vectors
- `reduce()` – Reduce a list to a single value

**Learn:**
- Using `map()` for iteration instead of loops
- Handling nested lists
- Functional programming concepts

---
### 6. tibble (Modern Data Frames)
**Key Functions:**
- `tibble()` – Create tibbles
- `as_tibble()` – Convert to tibble
- `glimpse()` – View data structure
- `print()` – Display tibble with control over rows/columns

**Learn:**
- Differences between tibbles and data frames
- Efficient data handling in R

---
### 7. stringr (String Manipulation)
**Key Functions:**
- `str_detect()` – Detect patterns in strings
- `str_replace()` – Replace text
- `str_extract()` – Extract substrings
- `str_split()` – Split text into parts

**Learn:**
- Handling and cleaning textual data
- Regular expressions (`regex`)
- String transformations

---
### 8. forcats (Factor Handling)
**Key Functions:**
- `fct_reorder()` – Reorder factor levels
- `fct_lump()` – Group rare categories
- `fct_inorder()` – Maintain factor order
- `fct_rev()` – Reverse order

**Learn:**
- Managing categorical data
- Reordering factor levels dynamically

---
## 📌 Supporting Packages

### 9. lubridate (Date & Time Handling)
**Key Functions:**
- `ymd()`, `mdy()`, `dmy()` – Parse dates
- `hms()`, `hm()` – Parse times
- `interval()` – Time intervals

**Learn:**
- Parsing and manipulating dates
- Handling time zones

---
### 10. hms (Time-of-Day Handling)
**Key Functions:**
- `hms()` – Create time-of-day objects
- `as_hms()` – Convert to hms format

**Learn:**
- Time-of-day calculations
- Formatting timestamps

---
### 11. magrittr (Piping)
**Key Functions:**
- `%>%` – Pipe operator

**Learn:**
- Chaining operations for cleaner code

---
### 12. modelr (Modeling Support)
**Key Functions:**
- `add_predictions()` – Add predictions to a dataset
- `add_residuals()` – Compute residuals

**Learn:**
- Integrating models with tidy workflows

---
### 13. broom (Tidy Model Output)
**Key Functions:**
- `tidy()` – Convert model output to tibble
- `glance()` – Get model summaries

**Learn:**
- Cleaning up model outputs
- Extracting insights from models

---
### 14. tidytext (Text Mining)
**Key Functions:**
- `unnest_tokens()` – Tokenization
- `bind_tf_idf()` – Compute TF-IDF

**Learn:**
- Text data analysis
- Sentiment analysis

---
### 15. glue (String Interpolation)
**Key Functions:**
- `glue()` – Construct strings dynamically

**Learn:**
- Efficient string formatting

---
## 📌 Learning Path

1. **Start with dplyr** – Practice filtering, selecting, and summarizing data.
2. **Move to ggplot2** – Learn basic and advanced plotting techniques.
3. **Understand tidyr** – Reshape messy data for analysis.
4. **Explore readr** – Import/export data efficiently.
5. **Apply purrr** – Master functional programming in R.
6. **Work with stringr & forcats** – Clean textual and categorical data.
7. **Delve into lubridate** – Handle dates and times effectively.
8. **Experiment with other packages** – Use advanced features as needed.

Happy Coding! 🚀
