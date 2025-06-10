## Ecosystem Model Design
Here's a breakdown of the key components of our ecosystem model:

## Environment
Our model simulates a 2D world grid. Each individual patch within this grid has the capability to grow food. The food supply is limited, and it serves as the primary energy source for the preys. After a fixed number of ticks, consumed food automatically regrows on its respective patch, simulating natural replenishment.

## Movement
Both preys and predators move randomly, employing a combination of "right random" and "forward" movements. Every movement incurs an energy cost. Both agents die when their energy reaches zero, emphasizing the importance of energy management for survival. They are initialized with a limited amount of starting energy.

## Predators
Predators actively search for preys, prioritizing those within their vision range or on nearby patches. When a predator successfully eats a prey, it regains a quarter of its initial energy. They consistently lose energy with each movement. Predators have a fixed probability to reproduce, contributing to the growth or decline of their population. Each predator possesses an energy variable that tracks its current energy level.

## Preys
Preys primarily search for food on patches. Upon eating food, they regain a quarter of their initial energy. Similar to predators, preys also lose energy per movement. They, too, have a fixed probability to reproduce, allowing their population to grow. Each prey agent maintains an energy variable to monitor its energy status.
