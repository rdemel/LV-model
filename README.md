# LV-model
LV model attempt to simulate competition between resistant and sensitive bacterial populations in the presence of an antibiotic

## Description

This a project for the SABS modelling and scientific computing module. This is an attempt at making a Lotka-Volterra model that simulates competition between resistant and sensitive bacterial populations.

Lotka-volterra model is a model made of a collection of nonlinear differential equations that is used to describe the relationship between two biological entities It is usually applied to prey and predator interactions but it can be modified to describe the dynamics of a slightly different nature, like in this case, resistant against sensitive bacterial populations in a closed system in the presence of an antibiotic.

Model assumption:


- Homogenous mixing of the resistant and sensitive bacterial populations plus antibiotic
- Parameters are constant
- Environment is constant
- DeltaA: The degradation rate of the antibiotic is constant- which is very wrong as this constant does not take into account antibiotics with a minor secondary mechanism of action, pharmacokinetics, environmental degradation and potential active metabolites.

## Parameters of the model

#Parameters of the equation:

rR, the growth rate of the resistant population-
S, the growth rate of the sensitive population-1
KR, the carrying capacity of the resistant population- 10,000
KS, the carrying capacity of the sensitive population- 10,000
AlphaRS, the competition coefficient representing the effect of the sensitive population on the growth rate of the resistance population-1
AlphaSR, The competition coefficient representing the effect of the resistant population on the growth rate of the sensitive population-1
AlphaR, the effectiveness of the antibiotic against the resistant population
AlphaS, the effectiveness of the antibiotic againsts the sensitive pop.
Mu, the mutation or acquisition rate at which sensitive bacteria become resistant
DeltaA, the degradation rate of the antibiotic concentration over time

## Installation

Can clone this repository or download this file as a py file and run it on your computer.

