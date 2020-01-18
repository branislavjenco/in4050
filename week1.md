# Week 1

## Machine learning
ability of a program to learn from experience
## Generalization
provide sensible outputs for inputs not encountered during training

## When to use ML?
- no human expertise
- unexplainable human expertize
- solutions are dynamic
- complex, large data
- noisy data

## Learning problem
Improve over task `T` with respect to some performance measure `P` based on experience `E`

## Reinforcement learning
The algorithm is told when his answer is wrong but _not how to correct it_


## Decision trees
- kind of a flowchart, answering one question at a time, moving forward to the next question
- can be used in _rule-based_ approaches (series of `if-else` statements`)
- can be learned from data

### Decision trees from data
- obtain data with several features (survey questions)
- find the best tree for this data => NP-complete => use a _greedy_ approach = always pick question which is most informative
- most informative = maximize ratio of majority class (simplified, otherwise look up ID3)

### Decision trees properties
- very explainable
- good for categorical data, can handle numerical
- not great for many features
- generalization = _random forests_
