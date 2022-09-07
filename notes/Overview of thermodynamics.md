---
title: Overview of thermodynamics
description: Overview of thermodynamics
parent: Notes
nav_order: 1
---

# Overview of thermodynamics
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Think of the systems and processes typically used to illustrate thermodynamics: the expansion and compression of gases, the mixing of dilute solutions, the stretching of rubber bands, and the reversible cycles of a working fluid that operates as an engine. The systems are macroscopic, at equilibrium, and slow moving.

## Definition

_What is thermodynamics?_
Thermodynamics is a (timeless) theory of the behavior microscopic systems that predicts how they exchange energy with each other or their environment.
Thermodynamics consists of rigorous rules about what processes are possible and which are impossible. For example, if we are interested in a particular chemical reaction, will that reaction proceed spontaneously?
These rules are set of laws based on experiments, each introducing a new concept or new observable.
While molecular interpretations are often helpful for understanding, its traditional form, there are no assumptions about molecular properties or intermolecular forces.

## Central problem

_What is the central problem of thermodynamics?_
The _central problem_ is to predict the equilibrium state that results after removing a constraint (e.g., free expansion of a gas).
With the ability to solve this _central problem_, thermodynamics can set ultimate limits on energy efficiency of reversible, infinitely slow processes (e.g., heat engine).
And, from predictions of efficiency, we can increase the amount of work that systems can perform.
The principles of thermodynamics were inspired by the desire to maximize efficiency and to scale up engines to do increasing amounts of work.

## Key features

_How do we use thermodynamics?_
We use thermodynamics to make predictions about the spontaneity of chemical and physical processes, to determine the maximum work that can be done by a system (free energies), to set bounds on the ultimate efficiency of natural processes, and to identify the states are matter that are most stable under some experimental conditions.
These features make thermodynamics useful for designing chemical and physical systems.

Another useful feature of thermodynamics is that it consists of relationships between observables. These relationships let us find a property we need by measuring one that's more convenient (and then use thermodynamic equations to convert). For example, we can find changes in the internal energy of the system, $$\Delta U = q + w$$, by measuring the energy exchanged as heat, $$q$$, and work, $$w$$, between the system and surroundings.

Together with statistical mechanics, thermodynamics gives us a framework to predict the properties of macroscopic systems using spectroscopic measurements (rotational constants, vibrational frequencies) or molecular calculations (ab initio quantum, semi-empirical, etc.).

## Example - Isothermal expansion of an ideal gas

As an example, you might remember the infinitesimal work done by the isothermal expansion of an ideal gas is: $dw_{\textrm{rev}}=-PdV$.
By integrating, we find the measurable amount of work in the expansion from $V_i$ to $V_f$: $w_{\textrm{rev}}=-\int_{V_i}^{V_f} PdV$.
We can evaluate the integral using the equation of state, $PV=nRT$, and the isothermal conditions to get:

$$w_{\textrm{rev}}= -nRT \ln\frac{V_f}{V_i}.$$

The internal energy of the ideal gas only depends on temperature. Since temperature is fixed, $\Delta U =0$, so that $q=-w$ and:

$$q_{\textrm{rev}} = -w_{\textrm{rev}}= +nRT \ln\frac{V_f}{V_i}.$$

If we use the thermodynamic definition of entropy, $dS = \delta q_{\textrm{rev}}/T$, then:

$$\Delta S = \frac{\delta q_{\textrm{rev}}}{T}= +nR \ln\frac{V_f}{V_i}.$$

From these relationships, we can see that we can measure the work (for the ideal gas under isothermal conditions) and predict the entropy change.

This example also highlights an important feature of thermodynamic observables.
The result above suggests the _absolute_ entropy of the initial and final equilibrium states is:

$$S = +nR \ln V/n = +Nk_B \ln V/N.$$

and that the entropy is _extensive_ -- it is of the order of the number of molecules $\mathcal{O}(N)$. The last equation in terms of the number of molecules, $N$, and Boltzmann's constant, $k_B$, comes from using $Nk_B = nR$.
Notice that both of these expressions have physical dimensions in the argument of the logarithm, so we have to consider entropy differences.
