# Thermal Physics
Here is some writing about some key ideas in Thermal Physics

### Equilibrium State and State Variables
An equilibrium state of a system is one where we can reasonably describe the system with its few bulk parameters. The system properties of the system (the state variables) need to be homogenous throughout the system for us to be able to describe it in this way. For example, if a gas were to have a position-dependent temperature, we wouldn’t be able to describe the gas with the parameters pressure and volume. This is because pressure would essentially be a function of position, rather than a straightforward ‘number’ describing the gas at large. This is in contrast to volume: the volume of the gas is simply a number, which describes the gas as a whole. It wouldn’t make sense to talk about a “position-dependent volume”, since volume is a property of the gas as a *whole*.

### Function of State
A **function of state**, or **state function**, is a property of a system which can be defined using only the equlibrium state of a system, via the associated state variables. For example, if we have a gas in the state (P, V), then F = P V + a P (for some constant a) is a function of state, as we can define it using the state variables of the system and nothing else.

If we are describing the system of people in the library, we can say that the number of people in the building is a state variable, since this depends only on the people currently inside the library and nothing else. The cummulative height of everybody in the library is a function of state, since it depends only on the state of the library. However, the identity of the last person to enter the library is _not_ a function of state, since this depends on _how_ the library got to the state where it is currently, rather than solely on its state.

The population of Scotland is a function of state, since we can look at Scotland and know this. However, the number of people who have _ever_ lived in Scotland is not a function of state, since we cannot possibly know this just by looking at Scotland at any given moment.

### State Function vs State Variable
State functions and state variables are sometimes essentially the same thing, in that they depend on how the system looks at a particular moment. For some quantities, we use the word 'variable' rather than the word 'function' to suggest a more fundamental role in describing the system, and/or a greater degree of direct control. For example, we could describe the state of a gas by its pressure and volume squared. The volume squared is equally as good at describing the system as the volume, and so we might wish to use the square volume as a state 'variable' instead of the volume. However, we generally won't do this, since we want to suggest that volume is more 'fundamental' than square volume, and we can more directly control this. However, since there is a one to one correspondence between volume and square volume, square volume would work equally as well as a coodrinate in describing the state.

However, if A is some fixed reference volume, the function sin(V/A) is **strictly** a function of state, and not a state variable. The reason for this is that many possible volumes V correspond to any given value sin(V/A). However, if the quantity of "volume" wasn't of interest to our system, we perhaps could talk about sin(V/A) as a state variable, rather than a state function: this would only work when we don't consider volume as an important feature in the state of our system. Basically, there is a subtle difference between functions of state and state variables, and these notions may sometimes overlap where it is convenient.

We may also view a state variable as a function of state of itself, where convenient!

### Adiabatic/adiathermal and diathermal
A rigid wall connecting two systems is said to be **adiabatic** or **adiathermal** if a thermodynamic changes in the systems are completely independent of each other. For example, if we changed the pressure or the temperature of one of the systems, the other system would not change. Note that the wall must be rigid, to avoid work being done.

A rigid wall which is not adiabatic is said to be **diathermal**.

### Thermal equilibrium
When we put two closed systems of gas in thermal contact with each other, their pressures and volumes might change. These quantities shall tend to settle down and approach constant values. In the limit of large times, where each gas is in an equlibrium state, we say that the gases are in **thermal equlibrium**. Essentially, we say that two systems are in thermal equlibrium when they have been in thermal contact in the limit of large time.

We observe experimentally that if systems A and B are in thermal equlibrium, and systems B and C are in equlibrium, then systems A and C are in thermal equlibrium. In other words, thermal equlibrium is transitive. One might be confused as to how we can _tell_ that systems A and C in this context are in thermal equlibrium, without leaving them in thermal contact for a long time. To solve this, we must have an experimental setup which can take two systems and tell whether or not they are in thermal equlibrium. Given that bringing the systems in to thermal contact for a large time puts the systems in to thermal equlibrium by definition, rather than checking if they are, how to go about this may seem unclear. However, given the discussion above, a clear experimental check for thermal equlibrium would be to bring two closed systems in to thermal contact with each other, and see if their pressures and volumes change. If they do, then the systems are _not_ in thermal equlibrium, whereas if they don't, the systems _are_ in thermal equlibrium.

We would say that a system is always in thermal equlibrium with itself, and that thermal equlibrium is a symmetric relation, and so thermal equlibrium is in fact an _equivalence relation_. We can partition every thermodynamic system in to equivalence classes based on this relation.

### Temperature
Recall from the discussion of Thermal Equlibrium that we can partition every thermodynamic system in to equivalence classes, induced by the relation of thermal equlibrium. We define temperature as a characteristic of each equivalence class. Mathematically, I suppose temperature is a function on the set of these equivalence classes. We have not yet decided whether this function is injective, nor have we decided what set the function actually maps in to.

This is similar to my favourite example of partitioning a set according to an equivalence relation. We might partition the set of all people in the library according to the relation "x is related to y if and only if x is the same age as y". We then have our partition, the sets of which consist of people all of whom are the same age. This is just like how we had our partition of all thermodynamic systems, the members of each set all being in thermal equilbrium. We then assign each equivalence class of people a characteristic: the age of each member. In a similar vein, we assign each equivalence class of thermodynamic systems a temperature!

### Equation of State
An equation of state is a constraining relationship between state variables/functions. The canonical example of an equation of state is the ideal gas law PV = nRT.

### Absolute Thermodynamic Temperature Scale
We can build a temperature system in a linear fashion. Let X be some quantity which varies with temperature (such as the height of mercury in a thin column). Then, choose a fixed point (like the triple point of water), and record the value of X at this point as X0. Then, define the X temperature scale with respect to your fixed point as T = c X / X0, where c is some scaling constant. In this regard, we _define_ temperature as this essentially linear quantity, which can make our equations look nice. However, I'm not sure if it is a sensible question to ask whether or not temperature really 'is' linear, whatever that might mean!

If we are using this temperature scale, and define values of temperature in this way, then we shouldn't be surprised if we find that the height of mercury is proportional to temperature, since we _defined_ temperature in this way! Seeing that mercury behaves in this way is completely uninteresting and tautologous, since the proportionality is literally built in to our definition of temperature.

If we use a different material instead, like steel, to define our temperature system as above, then we would expect to find that the length of steel is proportional to temperature, and we wouldn't necessarily be able to say the same about mercury anymore. I suppose the genuinely interesting things we do in physics are looking in to how these scales relate to each other! At reasonable temperature ranges, I guess we find that both mercury and steel have length proportional to temperature, no matter if we defined the temperature using mercury or steel!

We can see that temperature exists more abstractly from any temperature scale! In a similar way, the positions of objects exist more abstractly from their representation in any coordinate system, and distances between objects exist more abstractly from their representation in any system of distance (be it linear or non-linear). This reminds me somewhat of my discussion about axes and coordinates, in my tex file I wrote over the holidays.

### Processes
Thermodynamic systems change via _processes_. The state of the system at the beginning of a process is called the _start point_, and at the end is called the _end point_.

### Quasi-static Processes
A quasi-static process is a process which can be approximated by a succession of equlibrium states. This might seem paradoxical, since how can the system be in an equlibrium state (where the state variables are independent of time) as well as dynamically changing with time? However, by this, we mean: let the system be at a particular state. Then, given a difference in the state variables (epsilon), we can find a time interval (width delta t) such that for all times in this interval, the system's state variables are epsilon close to their values at the point we picked. If this holds for every point on a process, then the process is quasi-static. This basically reads as: close times have close states. In fact, this is essentially the definition of continuity from mathematical analysis! Perhaps reversible processes are those for which the state variables are continuous functions of time.