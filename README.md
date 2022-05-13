# Chicago-Public-School-Science-Assessment-MiniProject
Analyzing science assessments results from Grade 5, Grade 8, and HS Biology students in the Chicago Public School system.


Dataset: Chicago Public School Assessmnet Reports (attatched in repository)

The objective of this project was to explore the science assessment results from all Chicago public schools.
Python was used to read, clean, and store an XLS file.

# Observations: 4 Years of Data

- There is a strong negative correlation with Year and Overall Mean Score for all grade levels, ie. each year, students are scoring lower: R = -.758 with a P Val = .004. 
- Over 72,537 English as a Second Language Students: The relationship between Overall Mean Score and students with English as a second language had a -.952 R Score with a P Value of 1.79e^-25. The correlation with % Not Proficient had a R of .834 with a P Value of 1.71e^-13.
- Over 237,562 Economically Disadvantaged Students: The relationship between Overall Mean Score and students with Economic Disadvantage had a -.96 R Score with a P Value of 1.05e^-13. The correlation with % Not Proficient had a R of .805 with a P Value of 2.04e^-6.
- Over 143,852 Female Students: The relationship between Overall Mean Score and Female students had a .358 R Score with a P Value of .085. The correlation with % Not Proficient had a R of -.12 with a P Value of .574 (Both relationships are not significant).
- Over 28,414 White Students: The relationship between Overall Mean Score and White students had a .403 R Score with a P Value of .00014. The correlation with % Not Proficient had a R of -.35 with a P Value of .001.
- Over 100,301 Black Students: The relationship between Overall Mean Score and Black students had a -.639 R Score with a P Value of 5.99e^-11. The correlation with % Not Proficient had a R of .544 with a P Value of 8.859e^-8.

Unsurprisingly (and unfortunately), students with economic disadvantage, english as a second language, and black students all score lower and have a higher non proficiency percentage on the annual Science assessment for Chicago Public Schools. 

White students score higher and have a higher % of proficiency and female students did not have a statistically significant relationship with test scores.

Students are trending lower in overall mean scale score.

# Install
pip install numpy | conda install numpy

pip install pandas | conda install pandas

pip install matplotlib | conda install matplotlib

pip install seaborn | conda install seaborn

pip install scipy | conda install -c anaconda scipy

pip install plotly

pip install cufflinks

pip install chart-studio

# Import
import numpy as np

import pandas as pd

import matplotlib.pyplot as plt

import seaborn as sns

%matplotlib inline

import scipy.stats as st

import plotly

import cufflinks as cf

from plotly.offline import download_plotlyjs, init_notebook_mode,plot,iplot

init_notebook_mode(connected = True)

import chart_studio.plotly as py

cf.go_offline()
