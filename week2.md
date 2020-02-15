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

## Optimization methods
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





