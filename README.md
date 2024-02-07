# AI-BinPackingProblem-A1
Population Initialization: The population is initialized randomly, with each individual being a binary string of length string_length.

Fitness Function (fitness): Calculates the fitness of an individual as the sum of its bits. The aim is to maximize this sum, which means having as many 1s in the string as possible.

Parent Selection Function (select_parent): Implements roulette wheel selection. higher fitness values will be favoured as parents

Crossover Function (crossover): Performs a one-point crossover between two parents to produce two children. Each child inherits a part of each parent's string, split at a random crossover point. The crossover occurs with a probability defined by crossover_rate.

Mutation Function (mutate): Introduces variability into the population by flipping bits of an individual with a probability defined by mutation_rate. It helps the algorithm to explore the solution space and prevent premature convergence.

Evolution Function (evolve): It involves: Selecting parents. Performing crossover to produce offspring. Applying mutation to the offspring. Forming a new population from the offspring.

Execution Loop: Evolves the population for a number of generations defined by max_generations. In each generation: The population is evolved using the evolve function. The average fitness of the population is calculated and stored. The average fitness of the current generation is printed.

The code genrally follows this structure for all parts but some functions are different based on requirements (Specific Target String, Deceptive Fitness)
