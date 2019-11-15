# project goal and details 

*Authors: Liubov Tupikina, Bastian Greschake, Marc Santolini* 

The project is dedicated to analysis of mobility data for social good: "what we can learn from our geolocation about how people are traveling and how they can contribute to local communities around the globe". 
The research questions here are: 
1. What are the properties of mobility data: 
how can be characterize and predict future patterns of human mobility (e.g. geolocation data)?
2. How different factors (e.g. weather, population size, city network and distribution of bikes stations  etc.) 
can influnece mobility? E.g. how these factors may influence bike sharing functionality, public transport usage.

General question: how people are traveling between or within the city? Can we identify bottlenecks from the data of places, where people would like to go, but do not go for some reason?

# data collection 
If you are interested in contributing in data collection for traveling researchers, feel free to participate in the OH subproject on mobility of researchers https://www.openhumans.org/activity/mobility-data-of-researchers/


# datasets
Here we analyze two datasets: 
1. global mobility data 
2. individual mobility data 
There are many othttps://www.kaggle.com/dryad/human-mobility-during-natural-disasters datasets for analysis of trajectories such as https://crawdad.org/epfl/mobility/20090224/ or recently release Kaggle 
3. dataset for mobility of researchers https://www.openhumans.org/activity/mobility-data-of-researchers/
4. dataset examples https://github.com/mmalekzadeh/motion-sense/blob/master/Public_HAR_Data.md

# notebooks for analysis of individual trajectories

### notebook mobilitydata analyzer.ipynb
a. global mobility data (air planes) 
Open mobility data (accessed June 2019)
https://bluehub.jrc.ec.europa.eu/migration/app/index.html?state=5cc845a97758cd17cdecd1fb

We also are using great open data from openflights https://github.com/jpatokal/openflights/tree/master/data


We make analysis of mobility patterns of humans from various data sources and try to fit it to models 

### notebook Analysis of human mobility trajectories.ipynb
b. human mobility data from Openhumans open data from www.openhumans.org  
and inspired from notebooks from https://github.com/gedankenstuecke Open Humans

I also analyse later Erasmus network of student exchanges. 
Erasmus travels is a subnetwork of the first network a., since most of the time 
students are taking flights while travelling. 

### notebook analysis_of_trajectories.ipynb
We analyze random trajectory (can be uploaded from the file or can be randomly generated) using standard methods of stochastic processes.

The questions we consider here are:

1. How to analyze human moves, while not having the full access to trajectories and additional information about who is traveling?

2. How random is human trajectories?
Given the network of flights (nodes in this network are airports, links are connecting flights between them)
we can consider people to be represented by random walks on such network.
Then the random walk can be considered as an underlying model for 
dynamics on network of flights connections.
For random walk discovering networks see seminal work Modern Graph Theory | Bela Bollobas | Springer

3. Finally we are interested in the groups of humans traveling on a network. 
For this we can do a trick and consider random walk on a percolated underlying network of underlying human travels. 
The questions here are:

“What is the probability of a human being travelling a certain distance in a short period of time?” 
To more specific:
"How some specific people are travelling?"


# theoretical analysis of trajectories

We also fit the distributions to CTRW model. Important properties of CTRW are r(t) and d(t) distributions of lengths of jumps and durations correspondingly.

For more details look at code and papers here https://github.com/Liyubov/networks_random_walking 
More details are described for trajectories on networks: 

L. Tupikina, D.Grebenkov “Temporal and structural heterogeneities in networks” Applied network Journ. (2019) 

D.Grebenkov, L. Tupikina “Heterogeneous continuous time random walk”, link to Physical Rev. E Journal E 97, 012148 (2018)


Analysis of other dataset of roughly a million individual displacements was made here (work by D.Brockmann group)

http://rocs.hu-berlin.de/projects/wgproject/index.html 

They found that the dispersal of dollar bills can be described as follows.
The probability of traveling a distance in a short period of time days decays as a power law, i.e. p(r) \propto 1/(r^{1+mu}), mu =0.6.
This observation led to conjecture that the trajectories of dollar bills are reminiscent of Lévy flights, 
superdiffusive random walks characterized by a power law in the single step distribution. 


See also references: 

[1] Open mobility data (accessed June 2019)
https://bluehub.jrc.ec.europa.eu/migration/app/index.html?state=5cc845a97758cd17cdecd1fb

[2] Data (for travelling scientists) collected from Marie-Curie Alumni network survey (all data
are depersonalized privacy issues are separately discussed on the website of Lecturers without
borders)

[3] Data for social good https://osf.io/ph46f/ Lecturers without borders

[4] https://academic.oup.com/gigascience/article/8/6/giz076/5523201

[5] D.Brockmann group
http://rocs.hu-berlin.de/projects/wgproject/index.html 
