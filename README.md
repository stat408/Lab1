# Lab 1

Turn in one copy for each group, both as a word or PDF document and the R Markdown source file.

## Lab Overview

For this lab, you will be exploring a dataset containing housing sales in King County, Washington (the greater Seattle area). The intent of this lab is to get a feel for some of the basic features using tidyverse in R and explore this data set.

The entire lab will be worth 20 points. Please consider clarity of code and thoughtful writing with an emphasis on concise interpretations as each will be considered when grading labs.

## Questions
Answer the following questions in this R Markdown document. Please include code where necessary.

Download the Seattle Housing dataset, available at: [http://math.montana.edu/ahoegh/teaching/stat408/datasets/SeattleHousing.csv](http://math.montana.edu/ahoegh/teaching/stat408/datasets/SeattleHousing.csv).
```{r read.data}
library(tidyverse)
seattle_housing <- read_csv("http://math.montana.edu/ahoegh/teaching/stat408/datasets/SeattleHousing.csv")
```


#### 1. (4 points)
Describe the variables in the dataset. Select a few features in the data set that you think are relevant for determining housing prices. How might each of these influence housing prices?

#### 2. (4 points)
Use the `group_by()` function along with `summarize()` to create and print a new dataframe that contains summary statistics on housing prices. Write a short paragraph describing this dataframe.

#### 3. (6 points)
Using `ggplot2` create two figures with at least one showing the relationship between a two variable in the data set with the housing price.

#### 4. (4 points)
Summarize the take away points from your figures. These summaries should be 3-4 sentences and provide all of the context for your graphics so that an outside observer could understand the story you are illustrating.


#### 5. (4 points)
Choose a variable or set of variables and create a subset of homes from the entire the dataset. For example, consider homes with greater than 3 bedrooms. Then describe the differences between your selected subset of homes and the entire data set. You can do this with numerical summaries, graphical displays, and/or qualitative descriptions. 

#### 6. (3 points)
Based on what you have found in this data set, how might you model housing prices ($Y_{price} = ?$)? Note, I am not asking you to fit a model, but rather describe important relationships between the variables and housing prices. You may discuss statistical modeling techniques, but we will cover these later in the course.

