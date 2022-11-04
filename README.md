# Title: Probabilistic Causation - An account of the effectiveness of graph-based probability theory for causal analyses


## Objectives:
1. Analysis of causal relations using graph theory.
2. Represent features of football transfer market using a Directed Acyclic Graph (DAG).
3. Gather data from websites by webscraping.
4. Organize and preprocess data.
5. Perform probabilistic analyses using Bayesian probability.
6. From the proposed DAG, find the total causal effect of one variable upon the result variable.


#### Libraries used:
Pandas, NumPy, pymc3, Matplotlib, distfit, SciPy, sklearn


#### Data source:
Data fragments collected from ESPN, Transfermarkt and Soccerwiki and organized in pandas and MS Excel.


## Figures and tables
Fig 1: Proposed DAG (drawn on dagitty)
![](https://github.com/rud-ninja/Probabilistic_causation/blob/main/dag.jpg)



Fig 2: Boxplot of the features from the dataset showing outliers
![](https://github.com/rud-ninja/Probabilistic_causation/blob/main/boxplot.jpg)




Fig 3: A grid display of the correlation between football player performance and market value stratified by age group and team level.
![](https://github.com/rud-ninja/Probabilistic_causation/blob/main/correlations.jpg)




Fig 4: Posterior probability density curve of the variable age derived by Bayesian Inference technique (top) and distfit (bottom).
![](https://github.com/rud-ninja/Probabilistic_causation/blob/main/posterior.jpg) ![](https://github.com/rud-ninja/Probabilistic_causation/blob/main/distfit.jpg)





Fig 5: Final causal effects of players' performance on their market value.
![](https://github.com/rud-ninja/Probabilistic_causation/blob/main/finalprob.jpg)






For a comprehensive report on the principles, technique and results, please click [here](https://github.com/rud-ninja/Probabilistic_causation/blob/main/probabilistic_causation/probabilistic_causation_report.pdf) and then click on ***Football Transfer Market*** under *Research Objetives* in the Contents section.
