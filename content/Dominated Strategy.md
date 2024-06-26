---
tags:
  - game-theory
---
Relevant Courses: [[Game Theory]]

This is related to the idea of a [[Dominant Strategy]].

## Strictly Dominated Strategies

> [!summary] Definition: Strictly Dominated Strategy
> 
> A strategy $a_i \in A_i$ is **strictly dominated** by $a'_i \in A_i$ if
> 
> $$ u_i(a_i, a_{-i}) < u_i(a'_i, a_{-i}) \,\forall a_{-i} \in A_{-i}$$
> 
> In other words, no matter what actions other players take, the outcome / payoff of taking $a'_i$ is always better (and not equal to) taking $a_i$

Note that this can also generalize to any strategy $s_i$, not just action $a_i$.

### Iterated Removal of Strictly Dominated Strategies

With this property, you can use the following process: Iterated Removal of Strictly Dominated Strategies:

Assuming that every player acts [[Rationality (Game Theory)|rationally]], for any player, if any action they take is strictly dominated by another action or strategy, we can simply "eliminate" that action altogether—as there is no reason that the player would choose that action since they have a strictly better strategy. This simplifies our game.

## Weakly Dominated Strategies

> [!summary] Definition: Weakly Dominated Strategy
> 
> A strategy $a_i \in A_i$ is **weakly dominated** by $a'_i \in A_i$ if
> 
> $$ u_i(a_i, a_{-i}) \leq u_i(a'_i, a_{-i}) \,\forall a_{-i} \in A_{-i}$$ and
> $$ u_i(a_i, a_{-i}) < u_i(a'_i, a_{-i}) \text{ for some } a_{-i} \in A_{-i} $$
> 
> In other words, no matter what actions other players take, the outcome / payoff of taking $a'_i$ is the same or better than taking $a_i$, but is better in at least one scenario (they do not have exactly equal payoffs).

> [!info]
> 
> Weakly dominated strategies can still be [[Nash Equilibrium#Best Response|best replies]]: for a given set of actions that opponents perform, both $a_i$ and $a'_i$ could be the best response, since their payoffs are equal. Therefore, we can't use the same process of "[[#Iterated Removal of Strictly Dominated Strategies]]:" since a weakly dominated strategy could be a best response, it could also be part of a Nash Equilibrium. However, ***at least one equilibrium is always preserved*** (so the order of removal matters).

