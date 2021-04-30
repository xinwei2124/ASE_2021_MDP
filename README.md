# EvoPoli: Evolutionary-Guided Synthesis of Verified Pareto-Optimal MDP Policies

EvoPoli is a search-based software engineering approach and tool that supports the automatic synthesis of Pareto-optimal policies for MDPs with arbitrary combinations of constraints and optimisation objectives.

EvoPoli casts the synthesis of Pareto-optimal policies for MDPs as a multi-objective search-based problem and leverage the power of multi-objective generic algorithms to compute the required Pareto-optimal policies.


EvoPoli uses the probabilistic model checker [PRISM](prismmodelchecker.org) and is built on top of [EvoChecker](https://github.com/gerasimou/EvoChecker).


Instructions
------------

EvoChecker is a Java-based tool that uses Maven for managing the project and its dependencies, and for generating the executable jars.

EvoChecker uses under-the-hood JMetal 4.5 for multiobjective optimisation, PRISM 4.5 for probabilistic model checking, and Antl4 for parsing the probabilistic model templates.

1. Import the project in your IDE of preference

2. Set the following environment variable (In Eclipse go to Run / Run Configurations / Environment tab / New)
   > OSX: DYLD\_LIBRARY\_PATH = libs/runtime
   > *NIX: LD\_LIBRARY\_PATH = libs/runtime
   
3. Specify the configuration parameters in file [config.properties](https://github.com/gerasimou/EvoChecker/blob/newEvoChecker/config.properties)

4. Run
