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


## Short summary

Imagine a scenario in which a person lives in a forested area where there are several trees overhanging the power lines. At home, he has a fan in front of which he likes to sit and read books. The fan is connected to a device that looks like the speedometer in a car (a voltmeter) with a pointer that almost always points at a specific number. One day, he finds that the pointer has dropped to zero and smoke is coming out of the fan as its coil has blown up. He gets it repaired and the fan starts running again. On another day, he finds the fan has blown up again and the dial reading zero and therefore, he has to repair it again. This went on for a few weeks and every time his fan would start smoking, the dial read zero. He came to the conclusion that the fan blowing up was the cause the dial read zero. Much like the speedometer of a car when it comes to a halt. He finally gets tired of repairing the fan and decides just to enjoy nature's breeze. But still, he comes home one day and finds that the dial has dropped to zero, even when there was no fan to blow up. This was a startling discovery, and one that challenged his belief. On consulting his electrician who repaired the fan, he got to know the truth. The culprit behind the case of the mysterious dial and the burnt out fan was nothing but overcurrent. The thing that was responsible for both the fan blowing up and the pointer of the voltmeter dropping to zero.

This is a hypothtical example of when correlation between two things might be mistaken as causation. The relation between cause and effect is majorly regarded as systematic chain where one link is always followed by the next. The notion of probabilistic causation is that the cause-effect relationship is not that straightforward and where an observed effect might be attributed to several interacting causes. Any sort of analysis with a deterministic standpoint might be prone to bias (or confounding). This project observes cause-effect relationshhips as a network of several variables working in tandem to produce the final observed result (or lack thereof). We make use of graph theory to represent such relationships that help us identify confounding variable and colliders in the system and obtain the causal effect of one aspect over the final observation that is free from bias. The probabilistic nature of the the study gives some flexibility to the belief on occasions where the cause is *not* followed by the effect.

The particular scenario we have studied is that of football transfer market where it is often believed that a player's performance causes his market value to be whatever it is. We study all the different variables that might affect a player's transfer value and conclude whether the performance causes the market value to fall under a certain range. In our study, we find that it actually does but there are associated conditions as well.

## Figures and tables
Fig 1: Proposed DAG.

<img src="https://github.com/rud-ninja/Probabilistic_causation/blob/main/dag.jpg" alt="drawing" width="700"/>



Fig 2: Boxplot of the features from the dataset showing outliers

<img src="https://github.com/rud-ninja/Probabilistic_causation/blob/main/boxplot.jpg" alt="drawing" width="600"/>




Fig 3: A grid display of the correlation between football player performance and market value stratified by age group and team level.

<img src="https://github.com/rud-ninja/Probabilistic_causation/blob/main/correlations.jpg" alt="drawing" width="600"/>




Fig 4: Posterior probability density curve of the variable age derived by Bayesian Inference technique (left) and distfit (right).

<img src="https://github.com/rud-ninja/Probabilistic_causation/blob/main/posterior.jpg" alt="drawing" width="500"/>
<img src="https://github.com/rud-ninja/Probabilistic_causation/blob/main/distfit.jpg" alt="drawing" width="400"/>





Fig 5: Final causal effects of players' performance on their market value.

<img src="https://github.com/rud-ninja/Probabilistic_causation/blob/main/finalprob.jpg" alt="drawing" width="600"/>






For a comprehensive report on the principles, technique and results, please click [here](https://github.com/rud-ninja/Probabilistic_causation/blob/main/probabilistic_causation/probabilistic_causation_report.pdf) and then click on ***Football Transfer Market*** under *Research Objetives* in the Contents section.
