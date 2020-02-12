# Thermal Physics
Here is some writing about some key ideas in Thermal Physics

## The fundamental concepts

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

An example of a quasi-static process is slowly compressing an ideal gas from one volume to another. At each point along this process, the gas never leaves equlibrium. If we think back to the above note 'Equlibrium State and State Variables', this is equivalent to saying "at every point in this process, the state variables of the gas are always well defined". If instead we compressed the gas very quickly, then at the point of compression, the gas might not have a well-defined pressure. The 'local pressure' of the gas may vary from place to place as the gas recovers from the induced turbulence, and so there is a point where we cannot talk about *the* pressure of the gas.

The free expansion of a gas from a volume V1 to a larger volume V2 via the instantaneous removal of a partition wall is not a quasi-static process. At the instant where we remove the partition, we can argue that the gas does not have a well-defined volume!

### Work
Thermodynamic systems can transfer energy between each other via work. If I remember the subhonours thermal physics definition of work, it is "every energy transfer not related to a difference in temperature".

### Internal energy
It is found experimentally that for an adiabatic system, the work done in changing a system from one equlibrium state to another depends only on the start and end points of the process. For example, if we have a gas in the state (P1, V1) and wish to adiabatically change it to the state (P2, V2), the work depends only on the parameters P1, P2, V1 and V2.

Mathematically, we can construct a function from the ordered pairs of state variables to some set. In the above, we would have a function which takes ((P1, V1), (P2, V2)) as an argument, and returns what we shall refer to as a "work". Physically, we assert that f is anti-symmetric in its arguments. In other words, for all P1, P2, V1 and V2, f((P1, V1), (P2, V2)) = f((P2, V2), (P1, V1)). This corresponds to the fact that if we do W work to go from A to B, then we do -W work to go from B to A. This implies that the work done to go between a state and itself is necessarily zero.

For notational brevity, let's combine all the relevant state variables in to one symbol, say X. We now write the state (P1, V1) as X1.

>Actually, I suppose that this definition of work is the definition of a "conservative" work.

We can argue that f behaves associatively/transitively in the sense that f(X1, X2) + f(X2, X3) = f(X1, X3). Physically, this means that the the work done in going between two states is unchanged if we take a 'detour' via a third state, which is reasonable when value given by f depends only on the initial and final states.

The existence of such a well-behaved f implies that there exists a function g on A, which maps in to the same space as f. We can define g by fixing a state Y, and writing g(X) = f(Y, X). Observe that for any X1 and X2, we have g(X1) = f(Y, X1) = f(Y, X2) + f(X2, X1) = g(X2) + f(X2, X1), whereby g(X1) - g(X2) = f(X2, X1).

In our example with the gas, f is the work done when the system changes adiabatically from one state to another, and g is the internal energy. So, the internal energy is nothing other than the quantity derived from the adiabatic work!

### Heat
In the above discussion of work and internal energy, the work via which we defined internal energy was _adiabatic_: the system was thermally isolated. If a process takes a system from equlibrium state X1 to equlibrium state X2, then (per our definition above) the change in internal energy shall be exactly the same, being equal to the work required in the adiabatic case. However, in the non-adiabatic case, the work of the process will not be equal to the change in internal energy -- its particular value depends on the specifics of the process!

However, we shall always be able to tell what the difference between the work of a process and the difference in internal energy is. We can define quantity as Q = delta U - W, and refer to it as heat.

Of course, I could have defined the geat G and leat L, such that L + G = delta U - W, or maybe even that L^G = delta U - W. However, this would be a pretty inconvenient way to do physics. We want to choose quantities to work with which are as mathematically straightforward as possible! It seems conceptually more reasonable to think about _one_ quantity Q = delta U - W, rather than _two_, and especially unnatural to define them in a strange exponential way. The first law of thermodynamics looks so neat because we have constructed it to be so, at every single stage of our development.

The name heat is suggestive of some sort of 'thermal' energy flow. Perhaps we can make sense of this, it being a consequence of the system being allowed to interact with its environment in a way which does not involve work.

However, I think that personally I would rather have a bit more detail on why we use the suggestive word "heat" for this quantity. How can we understand heat? Is it really the flow of 'hotness', in some sense? I don't want to just take this for granted, since what then would the point in building this theory from the ground up be?

### Kelvin-Planck Statement of the Second Law
The Kelvin-Planck statement of the second law of thermodynamics is based on experimental evidence. Commonly referred to simply as the Kelvin statement, it reads

> It is impossible to construct a device that, operating in a cycle, will produce no other effect than the extraction of heat from a single body at a uniform temperature and produce an equivalent amount of work.

If the Kelvin statement were false, then we could see some bizarre behaviour of physical systems, such as computers powering themselves by extracting heat from their surroundings. A more succinct version of the Kelvin statement is

> A process whose only effect is the complete conversion of heat into work is impossible.

This is an equivalent statement since the word _only_ is included. If a gas expands isothermally, then the heat and work of the process cancel each other out: in other words, the heat supplied to the gas is converted completely in to work! However, this is consistent with the law, since the conversion of heat to work is certainly not the _only_ effect of this process: the gas is in a different state afterwards versus before!

### The Clausius Statement of the Second Law
The Clausius statement is a different formulation of the second law to Kelvin's. It reads

> It is impossible to construct a device that, operating in a cycled, will produce no other effect than the transfer of heat from a colder body to a hotter body.

This essentially means that a 'perfect refrigerator' is impossible to construct. In a similar fashion to our shortening of the Kelvin statement, we could rewrite it as

> A process whose only effect is the complete conversion of heat into work is impossible.

 If the Clausius statement were false, we would be treated to such absurdities as a pan of water boiling itself by cooling down the rest of the kitchen!
 
### Equivalence of the Clausius and Kelvin Statements
Since they are both said to be statements of _the_ second law of thermodynamics, we should hope that the Kelvin and Clausius statements are logically equivalent. We can see this by establishing that the negation of the Clausius statement implies the negation of the Kelvin statement, and vice versa.

Firstly, let the Kelvin statement by false. Then, we can construct a process which takes heat Q1 from a hot body and converts this completely in to work W = Q1 through a cycle. Now, we can use this work to power a refrigerator, drawing heat Q2 from a cold body and depositing heat Q1 + W = Q1 + Q2 in to a cold body. The net effect of this composite process is to draw heat Q2 from a cold body and deposit it in a hot body, which is a violation of the Clausius statement!

Conversely, let's suppose that the Clausius statement is false. Then, we can construct a process where work Q1 is drawn from a cold body and deposited in to a hot body. Let's try constructing a regular Carnot engine and using this to our advantage in making the engine convert heat entirely in to work. Say that the engine takes heat Q1 from a hot body, outputs work W, and so deposits heat Q1 - W into a cold body. We can them combine this engine with a process whose only effect is depositing heat from a cold body into a hot body, moving heat Q1 - W from our cold body into our original hot body. Since the net heat deposited into the cold body is zero, the overall effect of this composite process is the conversion of heat (from the hot body) _entirely_ in to work. But this is a violation of the Kelvin statement, and so the two formulations of the second law are in fact equivalent.


