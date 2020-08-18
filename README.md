# randomized_rounding_paper_code

This directory the code and the datasets used in the paper : Randomized rounding algorithms for large scale unsplittable flow problems.
It contains all the presented algorithm, functions to create the instances and already created datasets.
The code in this directory is Python3 code. A gurobi license is mandatory to use most of the solvers. The instances are stored using the pickle module of python.

create_and_store_instances.py
Contains functions to generate a custom dataset of instances

instance_mcnf.py
Contains functions to create graphs, commodity lists and thus create instances

launch_dataset.py
Contains functions to launch algorithms on a dataset with the multiprocessing python library

mcnf.py
Contains the MILP solver presented in the paper together with the function randomized_rounding_heuristic.
This function depending on the used parameters emulates all the randomized rounding algorithms presented in the paper : RR, SRR, CSRR, ...

mcnf_continuous.py
Contains the LP solvers, used to compute the linear relaxation of the unsplittable flow problem in the randomized rounding algorithms

mcnf_do_test.py
Enables to create custom instances and launch algorithms on them and plot the results

simulated_annealing.py
Contains the simulated annealing presented in the paper
