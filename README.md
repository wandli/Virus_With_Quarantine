## WHAT IS IT?

This model simulates the transmission and perpetuation of a virus in a human population.

It follows the idea of the SEIR model but adds a 'quarantine' factor.


## HOW IT WORKS

The model is initialized with 1000 people, of which 10 are infected.  People move randomly about the world in one of three states: healthy but susceptible (green), sick and infectious (red), not sick but infectious (yellow), and healthy and immune (gray). 

This simulation could model three conditions: no quarantine, secondary quarantine ( isolate all turtles who have interacted with infected ones), and tertiary quarantine (isolate all turtles who have associated with both infected ones and exposed ones).

An infected turtle needs at least 'cured-time' to become cured. It may become recovered at chance 'chance-recover' each day after cured-time. However, an exposed turtle always has a possibility of 'chance-recover' to become recovered. Once got infected, a turtle will die in the rate of 'death-rate'.

An exposed turtle has a possibility, 'exposed2infected-rate', of becoming infected during its exposed-duration. 

A recovered turtle is immune, which means it will never get infected again.

If a turtle is quarantined, it won't infect any other turtles. However, if a turtle is not quarantined before it transfers from exposed to infected, it costs 'accepted-time' days to become quarantined, for others may not know that it is exposed.


The simulation will stop if no one is infected or quarantined.


## HOW TO USE IT

Each 'tick' represents one day in the time scale of this model.

The 'infected-number' is how many turtles are infected initially. 'infectiousness' is how likely an infected/exposed turtle will affect others.

Populations of turtles in all states are shown in the graph 'Populations'.

You can set the variables mentioned above to change the conditions.
