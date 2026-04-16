---
date: '2026-02-01'
draft: true
title: 'Deriving the Heat Equation'
---

# Deriving the Heat Equation

The motivation for this post came from my complete lack of understanding during my first three weeks of my partial differential equations class, in which we jumped into deriving the heat equation on day one. I hope to help other students learning about mathematical physics who desire a less rigorous, but perhaps more explanatory, derivation of the heat equation. My understanding is based upon course lectures in PDEs by Dr. Ming Huo at the University of North Dakota and the following texts: *Applied Partial Differential Equations with Fourier Series and Boundary Value Problems* by Haberman, *Introduction to Partial Differential Equations with Applications* by Zachmanoglou and Thoe, *Partial Differential Equations of Mathematical Physics* by Sobolev, and *Elementary Differential Equations with Boundary Value Problems* by Edwards and Penney. As always, I appreciate error corrections.

### 1. What is the Heat Equation

One of the classical equations in mathematical physics is an equation that relates our physical theories of heat conduction to generalizable spaces, pioneered by Fourier. Such a tool allows us to model heat conduction of physical objects and predict outcomes given various conditions. 

### 2. Where to Start the Derivation

In mathematical physics, and other applied disciplines of mathematics, we derive equations from the principles of the subject we are modeling. So in physics, this means we take our physical theories as our guiding assumptions rather than any particular mathematical expression. In the case of the heat equation, we begin with our physical theory of heat energy, temperature, conduction, and the conservation of energy. Really, many of these ideas were being formulated at the same time as people were developing mathematical models to represent them; and in practice, the theories of physics and the mathematics emerge closely together. But given a physical theory and a task to derive an equation, we must start with the physical theory. 

### 3. Derivation

#### Assumptions

To make things simple, we will start from the simple one dimensional case, and then extend it to higher dimensions. 

So let's imagine heat conduction in a single dimension. Typically, we are told to imagine an arbitrarily thin rod. Whether it is imagined as straight or curved or twisted around doesn't matter so much for the moment, but it will later, so just imagine a straight rod. Since we want to know how this rod interacts at some endpoints, it will be convenient if we give it a length, $L$ , and we set a starting reference position along the $x$-axis at $x=0$. 

Now, let's ground several more assumptions. First, if we take an arbitrarily thin cross section of this arbitrarily thin rod, we will get an arbitrarily small cross-sectional area and volume; it needn't be a circular cross section, it can be any shape you want. However, we will assume this cross section has homogenous thermal properties. In other words, since we are attempting to model a one-dimensional thing, every point in a cross section ought to have the same properties, otherwise, this would imply that change is happening over another dimension. Essentially, we are making this arbitrarily thin cross-sectional object a point-like object. Next, for simplicity, let's assume that along the length of our one-dimensional rod, the thermal properties are homogenous. In other words, we don't have certain parts of the rod that behave differently than other parts of the rod: it is made of the same arbitrary stuff, so every equal cross section will have the same innate properties. Finally, for simplicity, let's assume that the surface along the length of the rod is perfectly insulated, so we are only concerned about heat conduction along the endpoints and along the rod itself. This ensures we are truly only considering one dimension of heat conduction, from position $x=0$ to position $x=L$. 

#### Definitions

With the ground assumptions laid for our object of study, we can now start defining mathematical models that we will use. First, let's make a function of heat energy. How do we do that? Well it's as easy as stating "suppose $e=$ heat energy." So now that we have a function of heat energy, does it provide any useful information? Is our model helpful? Hopefully it is apparent that our model is lacking some information. For example, does this function depend on any other variable, perhaps space, or time? If we again imagine our rod with the physical property of heat energy, and suppose this heat energy is unevenly distributed along the $x$-axis, then we can say that our function $e$ depends on $x$. We typically write this as $e(x)$. Similarly, if we imagine our rod over a span of time, we know the heat energy will conduct in some direction as time passes, thus, $e$ also depends on time, $t$. So we will say heat energy is a function of position and time and is represented as $e(x,t)$.  

Now, let's define the heat flux, that is, the movement of heat energy, to be $\phi (x,t)$, and let's define the function of all energy generated inside the rod to be $Q(x,t)$. This function of heat generation could be the result of myriad processes; maybe our rod has some sort of radiative heat from the interaction of its matter; maybe there is heat injected into it at some point. 

The physical theory of the conservation of heat energy will form the core of our derivation: The rate of change of heat energy per unit time is equal to the rate of heat flux out of all boundaries per unit time plus the heat energy generated per unit time. If we recall that rate of change is the derivative with respect to the dependent variable, then we can use our model functions to represent the conservation of heat energy as 

$$ \frac{\partial e}{\partial t}=\frac{\partial \phi}{\partial x} + Q$$.







