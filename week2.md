# Search and Optimization

## What we need for optimization
- a numerical representation _x_ for all possible solutions to the problem
- some kind of function _f(x)_ that tells us how good a solution _x_ is
- some way of finding max or min of _f(x)_ over _x_ 

## Types of optimization
- continuous - finding maxima and minima of functions
- discreete - finding an item with some properties among a collection of items

## Typical discreete optimization problems
- chip design
- timetabling
- travelling salesman

## Typical continuous optimization problems
- design of mechanical shapes
- economics - portfolio, risk management
- control systems

## Exploration vs Exploitation
![Exploration](exploration.png?raw=true "Exploration")
![Exploitation](exploitation.png?raw=true "Exploitation")
![Mix](mix.png?raw=true "Mix")

## Discreete optimization
### 1. Exhaustive search
- brute force
- test all possible solutions, pick the best
- guaranteed to find the best global solution
- can be approximated for continuous optimization as well, if we sample the space at regular intervals
- very slow (N! for TSP), so we usually use other methods that exploit the fact that search spaces have some structure and similar solutions are usually of similar quality
### 2. Greedy search
- generates and evaluates a _single_ solution
- modifies it to get closer to a local optimum
#### Hill climbing
- pick a random solution as current best
- compare to neighbouring solutions, if better, replace the current best
- repeat for some time
### 3. Simulated Annealing
- simulating a thermal process for obtaining low energy states
- set an initial temperature T
- pick an initial solution
- repeat:
  - pick a neighbouring solution
  - if the new one is better, keep it
  - otherwise, keep the new one with probability p that depends on the difference in quality and the temperature 
  - reduce T
## Continuous Optimization
### 4. Gradient descent/ascent
- because f(x) is continous, we can calculate the gradient - that tells us in which direction the function increases the most
  





