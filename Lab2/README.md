# Lab 2: Nim

## Introduction to the game and adopted strategies

Nim is a strategic mathematical game involving two players who alternate turns in removing, or "nimming," objects from separate piles. During each turn, a player is required to take away a minimum of one object, with the option to remove multiple objects, as long as they originate from the same pile. The objective of the game varies based on the version being played; it can be either to refrain from taking the final object or to be the one to take the last object. In our case the player taking the last object wins.

The lab has tasked us with develop a **rule-based agent** and an **evolutionary-based agent** able to play the Nim game.

## How it works

The main function (train()) implements an evolutionary algorithm with a population of genomes. In each iteration (generation), child genomes are generated by slightly modifying the parent genome. The child genome with the highest fitness replaces the parent genome if it surpasses its fitness. The process repeats for a specified number of generations. The variable save_parent determines whether the parent genome is replaced only if the child genome is better (in few words, if the solution is (1 + lambda) or (1, lambda)).
Every population changes its parent by a gaussian distributed variable, which can be determined a priori. In my algorithm, both sigma and mu are immutable.


## References

https://en.wikipedia.org/wiki/Nim

## Collaborations
I worked with: 
- Matteo Martini - s314786 (https://github.com/MatteMartini/Computational-Intelligence.git)
- Andrea Scaturro - s319480 (https://github.com/andrea-scaturro/Computational_Intelligence24.git)