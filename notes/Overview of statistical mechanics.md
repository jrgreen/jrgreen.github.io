---
title: Overview of statistical mechanics 
description: Overview of statistical mechanics
parent: Notes
nav_order: 2
---

# Overview of statistical mechanics
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Consider again the systems and processes typically used to illustrate thermodynamics.
The systems are macroscopic, at equilibrium, and slow moving.
However, they also consist of individual molecules.
So, let's take a _microscopic_ perspective.

The bulk properties of matter are "born" out of molecular motion and molecular structure.
We are interested in predicting the conditions under which chemicals react, substances dissolve, liquids mix and change phase, etc.

## Definition

_What is statistical mechanics?_
Statistical mechanics is a collection of physical models, mathematical equations approximations, and empirical laws to describe forces driving _molecular_ behavior and predicting _bulk_ behavior from it.
Like thermodynamics, it applies to chemical, biological, and physical systems.
In short, statistical mechanics relates the properties of individual molecules and their interactions to the empirical results of thermodynamics.

> The book by Dill and Bromberg has many good examples of unreasonable effectiveness of unrealistic simplifications (e.g., spherical molecules, molecules constrained to move on a discrete lattice).

## Central problem

_How do we connect molecular properties to thermodynamic properties?_
Answering this question is the central problem of statistical mechanics. Statistical mechanics relies on classical or quantum mechanics descriptions of molecules and their motion, and uses statistical methods to predict bulk properties/processes when number of molecules is large.
To put it simply, we want to average over microscopic arrangements to get thermodynamic observables.
We will need to review the essential ideas of statistics and probability.
With this central problem solved, we can potential design molecular properties and structure in order to optimize the deliver of work, the timescale of chemical reactions, the performance of an engine.

## Counting states

One, perhaps overly simplistic view, of statistical mechanics is that it consists of a set of methods for counting microscopic states, the spatial arrangements of the molecules in the system.
Consider a gas of classical molecules in a container at a fixed temperature.
A microscopic state is a "snapshots" of the system at one point in time. Another microscopic state is the "snapshot" at another time when the molecules have moved to new positions.
The number of these states, $W$, is extremely large.

You have probably seen _Boltzmann tombstone postulate_

$$S = k_B \ln W\quad \quad \text{or}\quad \quad W = e^{S/k_B}$$

which shows how the _absolute_ entropy is related to the number of states.
The number of states tends to grow as

$$W\sim e^{\mathcal{O}(N)}.$$

To check this statement and look at this connection between counting and thermodynamic observables more closely, let's consider a couple of examples.

## Example - Collection of dipoles

Take a dipole that can be oriented in one of two directions: up or down. A single dipole has only two possible states. A collection of $N$ dipoles, will exist in one of

$$ 2\times 2\times \ldots = 2^N = e^{N\ln 2}$$

microscopic states.
The last expression suggests $W\sim e^N$ with an exponent that has both an extensive part $N$ and an intensive part $\ln 2$.

## Example - Ideal gas at fixed temperature

If we take $N$ identical molecules to occupy the volume $V$, each molecule can explore the entire volume; the gas is ideal, so each molecule does not exclude the others from occupying its volume.
The molecules are independent and indistinguishable, so the number of states is

$$\frac{V^N}{N!}\approx \frac{V^N}{N^N} = e^{N\ln V/N}.$$

The last expression again suggests $W\sim e^N$ with an exponent that has both an _extensive_ part $N$ and an _intensive_ part $\ln V/N$.
Comparing this last result to the [thermodynamic entropy of an ideal gas]({{ site.baseurl }}{% link notes/Overview of thermodynamics.md %}#example---isothermal-expansion-of-an-ideal-gas), we see that the entire exponent is the absolute entropy, $S/k_B$. In other words, _counting microscopic states_ has led us to a property of _macroscopic states_, the entropy,

$$W = e^{S/k_B},$$

and the Boltzmann tombstone postulate, $S = k_B \ln W$.
