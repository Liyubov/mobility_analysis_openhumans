# mobility analysis
analysis of mobility patterns of humans from various data sources and models

# analysis of global mobility data
Here we analyze two datasets: 

a. global mobility data (air planes) 
Open mobility data (accessed June 2019)
https://bluehub.jrc.ec.europa.eu/migration/app/index.html?state=5cc845a97758cd17cdecd1fb


b. human mobility data from Erasmus network of student exchanges, and Openhumans open data from Openhumans.org  

Erasmus travels is a subnetwork of the first network a., since most of the time 
students are taking flights while travelling. 

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

See also references: 

[1] Open mobility data (accessed June 2019)
https://bluehub.jrc.ec.europa.eu/migration/app/index.html?state=5cc845a97758cd17cdecd1fb

[2] Data (for travelling scientists) collected from Marie-Curie Alumni network survey (all data
are depersonalized privacy issues are separately discussed on the website of Lecturers without
borders)

[3] Data for social good https://osf.io/ph46f/ Lecturers without borders

[4] https://academic.oup.com/gigascience/article/8/6/giz076/5523201
