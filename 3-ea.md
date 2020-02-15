Week 3 - Evolutionary Algorithms
===
- insipired by biological evolution
- lifeforms adapt to a particular environment over generations
- combination of traits that are betterr adapted tend to increase representation in population
- can be mimicked to solve complex problems
> Variation ~ Crossover, Mutation

> Selection ~ Survival of the fittest

# Two competing forces
- _increasing_ population _diversity_ by mutation, recombination ~> **novelty**
- _decreasing_ population _diversity_ by selection of parents/survivors ~> **quality**

# Terms
**Gene** - one element of an array

**Locus** - position of a gene

**Allele** - 0 or 1 - what value a gene can have

**Genotype** - set of gene values

**Phenotype** - what could be built/developed based on the genotype

# Components

![scheme of ea](ea.png?raw=true "Scheme of EA")

## Evaluation (fitness) function
- represents the task to solve
- enables _selection_
- assigns a real-values fitness to each phenotype

## Population
- candidate solutions (individuals) of the problem
- _population_ is evolving, not individuals
- selection operators act on population level
- variation operators act on individual level

## Selection mechanisms
- identify individuals to become parents
- identify individuals to survive
- pushes population to a higher fitness
- parent selection is probabilistic (stochasticity can aid escape local optima)

## Variation operators
- generate new candidate solutions
- types based on arity (number of inputs):
  - 1 - _mutation_ operators
  - >1 - _recombination_ operators
  - 2 - _crossover_
  - >2 - not used much

### Mutation
- cause small, random variance to a genotype
- randomness is _essential_

### Recombination
- merge information from parents into offspring
- choice of what to merge is stochastic

## Initialization
- at random, even spread of allele values
- can use existing solutions as seed

## Termination
- reaching some fitneses, or maximum allowed N of generations, some minimum level of diversity or reaching some specified number of generations that didn't lead to an improvement

# Representation
- most common representation of genomes: 
  - binary, integers, real, float, permutation, tree
- most difficult part of building an EA - choosing representation
- determines what kind of variation operators are used

## Binary
- genotype is a string of binary digits
- mutation = alter each gene independently with a probability of p<sub>m</sub> (mutation rate)
- crossover - two children
  - 1-point crossover - choose a random point on two parents, split and exchange tails
  - n-point crossover - choose n random points on two parents, split and alternate
  - uniform crossover - flip a coing for each gene for first child, inverse for the second
- crossover - explorative
- mutation - exploitative


