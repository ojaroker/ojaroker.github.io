---
layout: page
title: Optimal Harvesting
description: Stochastic Control of a Predator-Prey Fishery
img: assets/img/projects/predator_prey/illus.jpg
importance: 2
category: "2025"
related_publications: false
pdf: OptimalHarvesting.pdf
---

How should you fish two species at once when one of them eats the other? This project treats a predator-prey fishery as an optimal control problem. The two populations rise and fall in the usual boom-and-bust cycle, with random environmental variation on top, and the goal is to set harvesting rates for both species that maximize expected profit over a season — accounting for market prices and for the fact that fishing gets more expensive as a stock runs low.

The tricky part is that today's catch changes tomorrow's stock, so the optimal decision at any moment depends on the entire future of the system. Handling this properly leads to a pair of coupled equations, one running forward in time and one backward, which have to be solved together and numerically. Much of the work here went into getting that backward solve right, and into building checks that could actually catch it being wrong.

The most interesting result is a sign. The prey turns out to be worth more left in the water than caught today, so the optimal strategy fishes it less aggressively than short-term profit alone would suggest. The predator goes the other way: it is fished harder than the myopic rate even though it sells for more, because every predator left in the water eats into the prey stock. Harvesting the predator doubles as a way of protecting the prey, which is something a single-species model cannot tell you.

The simpler of the two noise models is solved and validated; a second version, where heavy fishing itself makes the ecosystem more volatile, is worked out on paper but not yet implemented. The paper is a working draft, and the MATLAB code is on [GitHub](https://github.com/ojaroker/OptimalHarvesting).
