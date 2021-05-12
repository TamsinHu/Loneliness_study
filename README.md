# Loneliness and Deprivation in England

This repository contains supplementary material for our coursework submission for the Advanced Data Science course (COMSM0056 2020/21).

## Code

Code for generating the models and visualisations can be found in the Jupyter notebooks in this repo.

## Acknowledgments

We would like to thank Laura Gemmell for being an awesome supervisor and the lecturers and our cohort's TA, Emily Vosper, on the Advanced Data Science course for teaching us so much. We shamelessly stole the colour scheme for the bivariate choropleth from [Joshua Stevens](https://www.joshuastevens.net/cartography/make-a-bivariate-choropleth-map/).

## Appendix A - IMD shorthand

The following table explains the shortcut labels used for the various indices of deprivation.

|Label | Explanation |
--- | --- 
imd                   | Index of Multiple Deprivation
income                | Income Deprivation
employment            | Employment Deprivation
education             | Education, Skills and Training Deprivation
health                | Health Deprivation and Disability
crime                 | Crime Deprivation
housing               | Barriers to Housing and Services
living                | Living Environment Deprivation
child poverty         | Income Deprivation Affecting Children Index (IDACI)
elderly poverty       | Income Deprivation Affecting Older People (IDAOPI)
young people skills   | Children and Young People Skills Sub-domain of Edu
adult skills          | Adult Skills Sub-domain of Education Deprivation
geographical barriers | Geographical Barriers Sub-domain of Housing
wider barriers        | Wider Barriers Sub-domain of Housing
indoor                | Indoors Sub-domain of Living Environment
outdoor               | Outdoors Sub-domain of Living Environment

## Appendix B - Random forest hyperparameters

The following table summarises the hyperparameters used by the different models after randomised search. In order, the parameters are: the maximum depth of the trees, the minimum number of samples that are required to create a leaf and the minimum number of samples requires to split a node.

### _Loneliness_ setting

Geographic area | max\_depth | min\_sample\_leaf | min\_samples\_split| 
--- | --- | --- | ---
Postcode | 90 | 4 | 10
Local Authority | 50 | 4 | 2 

### _Conditions_ setting

Condition | max\_depth | min\_sample\_leaf | min\_samples\_split| 
--- | --- | --- | ---
Depression | 30 | 2 | 5 
Alzheimer's | 50 | 2 | 10
Hypertension | 70 | 1 | 2
Insomnia | 90 | 2 | 5
Addiction | 90 | 1 | 5
Social anxiety | 100 | 0.1 | 0.1
