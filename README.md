## BST270_IndividualProject

### Purpose

This repository attempted reproduction of 2 figures from FiveThirtyEight's article
on the high age of congress: [Congress Today Is Older Than It's Ever Been](https://fivethirtyeight.com/features/aging-congress-boomers/).

### Running the project

All code is located in the R Markdown ./Code/reproducible_pipeline.Rmd. This
can easily be knit as an html document as is default. **pacman** is used 
for conditional loading or installation of necessary packages, and **here** is
used to manage directory structure. The code file will also create a `./Data`
directory if none exists and then populate it with the necessary congress
ages data from 538's [GitHub](https://github.com/fivethirtyeight/data/tree/master/congress-demographics)

### Production

The output html file will have some tabset toggling. The first section includes
a brief description of the project and a tab can be selected that includes
the 538 data README. The second and third sections includes an option for a static plot
or a dynamic one using plotly. Both were included, as 538's website has dynamic
plots, but the limitations of the current implementation of plotly made it 
impossible (or at least too difficult) to accurately replicate the visual 
formatting. The second section corresponds to the first figure, which shows median
age of the House and the Senate by year. The third section corresponds to the 
second figure which shows the proportion of each generation in congress by year.
