# Dynamic Precision Medicine - Code Repository
This Github Orgainzation Represents the hub for information on various research directions. 

## Dynamic Precision Medicine
Key features of DPM: Dynamic precision medicine (DPM), co-invented
by Dr. Robert Beckman and Dr. Chen-Hsiang Yeang, is a strategy that
prioritizes the elimination of these multi agent resistant subclones by
changing therapy very frequently and pro-actively planning for potential
future evolution 20 . Current precision medicine (CPM) customizes
therapy to average, static cancer properties, treats with the best
therapy for this average state until recurrence, and then tries to repeat
the process with a new therapy, with diminishing returns as each line of
therapy stops working. DPM explicitly considers minority subclones and
heritable genetic/epigenetic evolutionary dynamics, with the goal of
treating current disease and preventing refractory disease relapse by
blocking future acquisition of simultaneous resistance to multiple non-
cross resistant agents. (Notably, many agents do exhibit cross
resistance and DPM requires availability of at least two therapies with
limited cross resistance). As a result, DPM will often recommend
prioritizing elimination of rare hypermutator subclones vs. debulking the cancer.

Foundational Work: 

[Impact of genetic dynamics and single-cell heterogeneity on development of nonstandard personalized medicine strategies for cancer](https://www.pnas.org/doi/10.1073/pnas.1203559109)

## Evolutionary Classifier
Current precision medicine (CPM) matches patients to therapies using traditional biomarkers, but inevitably resistance develops. Dynamic precision medicine (DPM) is a new evolutionary guided precision medicine (EGPM) approach undergoing translational development. It tracks intratumoral genetic heterogeneity and evolutionary dynamics, adapts as frequently as every 6 weeks, plans proactively for future resistance development, and incorporates multiple therapeutic agents. Simulations indicated DPM can significantly improve long-term survival and cure rates in a cohort of 3 million virtual patients representing a variety of clinical scenarios. Given the cost and invasiveness of monitoring subclones frequently, we sought to determine the value of a short DPM window of only two 6-week adaptations (moves).

[Generalized Evolutionary Classifier for Evolutionary Guided Precision Medicine](https://ascopubs.org/doi/10.1200/PO.23.00714)

[Github repository](https://github.com/GU-DPM/EvolutionaryClassifier)

## DPM-J
Despite advances in targeted cancer therapy, the promise of precision medicine has been limited by resistance to these treatments. In this study, we propose a mathematical modelling framework incorporating cellular heterogeneity, genetic evolutionary dynamics, and non-genetic plasticity, accounting for both irreversible and reversible drug resistance. Previously we proposed Dynamic Precision Medicine (DPM), a personalized treatment strategy that designed individualized treatment sequences by simulations of irreversible genetic evolutionary dynamics in a heterogeneous tumor. Here we apply DPM to the joint model of reversible and irreversible drug resistance mechanisms, analyze the simulation results and compare the efficacy of various treatment strategies. The results indicate that this enhanced version of DPM significantly outperforms current personalized medicine treatment approaches. Our results provide insights into cancer treatment strategies for heterogeneous tumors with genetic evolutionary dynamics and non-genetic cellular plasticity, potentially leading to improvements in survival time for cancer patients.

[Personalized cancer treatment strategies incorporating irreversible and reversible drug resistance mechanisms](https://www.nature.com/articles/s41540-025-00547-5)

[Github repository](https://github.com/GU-DPM/DPM-J)


## Future Directions and Other (incomplete) work
This section describes projects currenly underway.

### Clinical Trail App
**Background:**
Dynamic Precision Medicine (DPM) is a therapeutic strategy that reframes cancer
treatment to maximize long-term survival by proactively managing tumor evolution
(Beckman et al., 2012). It provides a data-driven method for planning optimal therapy
sequences for individual patients. A key breakthrough is the Evolutionary Classifier
(EC), a novel predictive biomarker that identifies patients who will derive substantial
benefit from DPM, enabling a new biomarker-stratified clinical trial design (McCoy et al.,
2025). Further, a novel biomarker-stratified randomized clinical trial design for robust
evaluation of DPM is in review (Parashar et al., 2025).

**Problem statement:**
Conventional clinical trials for targeted therapies often fail to deliver durable responses
due to the inevitable evolution of drug resistance. This leads to costly late-stage failures
and limits long-term patient survival. We address this critical need for a strategic
framework that proactively manages tumor evolution to increase the probability of trial
success and demonstrate superior, long-term outcomes.

**Methods:**
We developed a user-friendly R Shiny app to simulate DPM clinical trials based on a
large in silico patient database. The tool allows users to vary key parameters—including
sample size, trial design, and EC definitions—to evaluate trial performance. Outputs
include simulated hazard ratios, statistical power, and Kaplan-Meier curves, providing a
platform for both statisticians and clinicians to explore DPM-based designs.

**Key findings:**
Simulations of 200-subject, 3-year trials demonstrated high statistical power, with over
79% of trials achieving >80% power across various designs. In the recommended
biomarker-stratified design, DPM achieved an average hazard ratio for overall survival
of 0.45 (95% CI: 0.28, 0.64) versus the current standard in the predicted DPM-benefit
group.

**Implications/importance:**
Our findings demonstrate DPM offers a transformative approach for Novartis's oncology
pipeline. The potential for a hazard ratio of 0.45 represents a profound improvement
over the standard of care and provides a compelling rationale for using later-line agents
earlier, expanding market potential. Critically, the Evolutionary Classifier (EC) enables
the enrichment of trial populations, facilitating smaller, faster, and more powerful pivotal
trials. This de-risks development and accelerates the path to approval. The R Shiny
application serves as a powerful decision-support tool for Novartis teams to simulate
and optimize DPM-based trial designs, maximizing asset value and competitive
differentiation.

Coming soon: code repository link

### Goldilocks Hypothesis
The Goldilocks Hypothesis is a framework for predicting treatment
effectiveness in controlling drug resistance.

It classifies patients based on their response to drug therapy into:

* Too-Easy Case: Resistance is mostly due to mutation.
* Too-Hard Case: Resistance cannot be prevented.
* Goldilocks Zone: The ideal treatment range, where resistance is
manageable.


### Digital Twin Processing
Development of a generalized code that performs analysis on simulation output objects (sets of parameters and associated survival statistics for alternate therapeutic strategies)

### pyDPM
Python implementation of DPM, used to build prototype tools for simulating individual patients from a user specified input parameters, and visualizing the simulatin results.

https://github.com/GU-DPM/Documentation

https://github.com/GU-DPM/python-simulation

https://github.com/GU-DPM/pyDPM-notebook

https://github.com/GU-DPM/pyDPM-parameter-notebook



### DPM Legacy Code
Original CodeCode authored by Chen-Hsiang Yeang.

Github coming soon.


